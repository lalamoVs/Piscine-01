Exercise 01:
Environment variable can be created by using this command:
export FT_USER=bocal
to call variable: 
>> echo $FT_USER

command: printf, groups, tr, Pipeline (|)
printf: Display a formatted string (Similiar in python)
groups: Display the groups user
tr: translate/replace/ characters from input
Pipeline (|): Additional execution

display a formatted string from a list of groups the user is belong to
printf "%s$>\n" "$(groups $FT_USER | tr ' ',',')"
keys: Display the string in front of "$>", finally break line (\n). '$' treated as variable string (%s). replace space to ","
