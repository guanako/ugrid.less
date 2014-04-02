lessc = lessc
browser = firefox

demo.css: demo.less ../ugrid.less
	@echo -n "Compiling..."
	@$(lessc) $< > $@
	@echo "done."

clean:
	@echo -n "Cleaning..."
	@rm demo.css 2>/dev/null || true
	@echo "done."

test: demo.css
	$(browser) demo.html &
