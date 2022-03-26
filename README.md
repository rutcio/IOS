# IOS
print_help()
{
    echo "Usage: corona [-h] [FILTERS] [COMMAND] [LOG [LOG2 [...]]"
    echo " "
    echo "LOG are files with records"
    echo " "
    echo "COMMAND:"
    echo "  infected — calculates the number of infected."
    echo "  merge — merges several files with records into one, preserving the original order."
    echo "  gender — vypíše počet nakažených pro jednotlivá pohlaví."
    echo "  age — lists the number of infected for each gender."
    echo "  daily — prints the statistics of infected persons for each day."
    echo "  monthly — prints the statistics of infected persons for each month."
    echo "  yearly — prints the statistics of infected persons for each year."
    echo "  countries — prints statistics of infected persons for each country of infection."
    echo "  districts — prints statistics of infected persons for individual districts."
    echo "  regions — prints statistics of infected persons for individual regions."
    echo " "
    echo "FILTERS:"
    echo "  -a DATETIME — after: only records after this date (including this date) are considered. DATETIME is of the YYYY-MM-DD format."
    echo "  -b DATETIME — before: only records before this date (including this date) are considered."
    echo "  -g GENDER — only the records of infected persons of a given sex are considered. GENDER can be M (men) or Z (women)."
    echo "  -s [WIDTH] — for the gender, age, daily, monthly, yearly, countries, districts and regions commands, it prints data not numerically,
            echo but graphically in the form of histograms. The optional WIDTH parameter sets the width of the histograms,
            that is, the length of the longest line, to width. Thus, width must be a positive integer.
            If the WIDTH parameter is not specified, the line widths are governed by the requirements below."
    echo " "
    echo "HELP:"
    echo "  -h — print a help with a short description of each command and switch."
    exit 0
}
