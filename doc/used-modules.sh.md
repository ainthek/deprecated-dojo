echo "

# Modules used on our project

This is only sample showing what we are using and not.



| mid | used | somehow deprecated |
|-----|------|------|
$(
	# our repo, out tools, you do not have this
	< "$INIT_REPO_DOC/04-tech/12-development/amd-aliases/amd-aliases.md" cut -d"|" -f2 |\
		trim | grep "^\(dojo\|dijit\|dojox\|util\)" | sed 's;[\\]_;_;g' | sort -u | sufix "\tYES" > used.txt

	< dojo-website/src/documentation/api/1.10/details.json jsontool -M |\
		jsontool -a key  | sufix "\tX" > all.txt
	< deprecated.txt  sed "1,2d" | cut -f1 | sufix "\tDEPR" > depr.txt
		
	join-paste all.txt used.txt depr.txt | grep -v "\." | awk -F"\t" 		'{print $1"\t"$3"\t"$4}' |\
			md-escape-emphasis | md-table | sed "1,2d"

	rm all.txt used.txt depr.txt
)


"