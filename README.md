A *simple* shell script to load up a Magento environment and execute PHP code
Very experimental and should only be ran on dev servers

REQUIRES 
  php pcntl

OPTIONAL
  php readline (no history, autocomplete or cursor support)

KNOWN ISSUES
ctrl+c doesn't exit app until you return/enter (but at least it'll save your history)
poorly written auto complete functionality
input must be able to be eval'd (e.g. `$x="` would cause a syntax error)


INSTALL
place in your include path or base magento directory, make sure it's executable
must be ran from base magento directory

USAGE
imc [store_code]

INFO
History File Saved at ~/.imc_history
Log File Saved at ~/imc.log
