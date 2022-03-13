all:
	yarn docs:build
	tar -czf dist.tar.gz .vitepress/dist
	scp dist.tar.gz liu1:/home/one/github/web3doc/dist.tar.gz
	rm -rf dist.tar.gz
	rm -rf dist
	ssh liu1 "cd github/web3doc;rm -rf pinia; tar -xzf dist.tar.gz; rm -f dist.tar.gz;mv .vitepress/dist ./pinia;rm -rf .vitepress"
