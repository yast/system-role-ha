
# checks only those control files that belong to this package
check: /usr/share/YaST2/control/control.rng
	xmllint --relaxng /usr/share/YaST2/control/control.rng --noout *.xml

# run "jing" to get more details about the validation errors
check-jing: /usr/share/YaST2/control/control.rng
	jing /usr/share/YaST2/control/control.rng *.xml
