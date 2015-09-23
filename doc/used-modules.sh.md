echo "

# Modules used on our project

This is only sample showing what we are using and not.

TODO: join modules with deprecated APIs

| mid | used |
|-----|------|
$(
	# our repo, out tools, you do not have this
	< "$INIT_REPO_MAIN/UI/gjax-tools-ui/src/main/sh/grasp/lib/amd-aliases.md" cut -d"|" -f2 |\
		trim | grep "^\(dojo\|dijit\|dojox\|util\)" | sed 's;[\\]_;_;g' | sort -u | sufix "\tYES" > used.txt

	< dojo-website/src/documentation/api/1.10/details.json jsontool -M |\
		jsontool -a key  | sufix "\tX" > all.txt

	join-paste all.txt used.txt | grep -v "\." | awk -F"\t" '{print $1"\t"$3}' |\
		md-escape-emphasis | md-table | sed "1,2d"

	rm all.txt used.txt
)


"