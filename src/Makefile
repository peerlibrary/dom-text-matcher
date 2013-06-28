default: compile

clean:
	rm -f *.js *.map

compile: clean
	coffee -m -c dom_text_matcher.coffee
	coffee -m -c text_match_engines.coffee

uglify: compile
	uglifyjs dom_text_matcher.js -c -m > dom_text_matcher.min.js
	uglifyjs text_match_engines.js -c -m > text_match_engines.min.js

