all: *.md
	mkdir -pv ../target
	cat components/header.html > ../target/`echo $^ | sed 's/md/html/'`
	php $^ | marked >> ../target/`echo $^ | sed 's/md/html/'`
	cat components/footer.html >> ../target/`echo $^ | sed 's/md/html/'`
