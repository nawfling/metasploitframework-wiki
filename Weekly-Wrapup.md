# Automated pieces for the Weekly Metasploit Wrapup blog posts

1. Clone https://github.com/egypt/metasploit-stats 
1. Run `get_release_notes.rb <start tag> <end tag>  >> ~/weekly.md`
1. Run `msf-wrapup.rb` in the `metasploit-framework` checkout:
   * `../metasploit-stats/msf-wrapup.rb <start tag> <end tag>  >> weekly.md`
1. Edit: `vim weekly.md`
1. Convert to html: `pandoc -f markdown -t html weekly.md`