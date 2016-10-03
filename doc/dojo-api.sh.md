
$(
< dojo-website/src/documentation/api/1.10/details.json jsontool --items |\
	jsontool -d $'\t' -a key value.type > modules.txt

< modules.txt grep -v "/_" > modules.public.txt 

)
echo "
# dojo-api 

Some statistics we can find from dojo api docs (detail.json)

## Modules count

| module | count |
|--------|-------| 
$( < modules.public.txt cut -d"/" -f1 | cnt | clmn-swap | trim | md-table " ")

## Types of modules
$(
	data=$(
		< modules.public.txt awk -F$'[/\t]' '{print $1" "$NF}' | sort | uniq -c
	)

	<<< "$data" md-indent
	<<< "$data" chart -c bar -B 100
)

## Cont of public methods of dojo/* modules

Definition:

        module.methods
        .filter(notDeprecated)
        .filter(notPrivate)
        .filter(notInherited, module) 

Data: 

$(
	data=$(
		./bin/dojo-api-public dojo-website/src/documentation/api/1.10/details.json |\
			cut -f1,2 | grep ^dojo/ | sort | uniq -c
	)
	
	<<< "$data" md-indent
)


"

$(
rm modules.txt modules.public.txt
)