mkdir repos
for i in *.md; do pandoc "$i" -o "repos/${i%.*}.rst"; done

