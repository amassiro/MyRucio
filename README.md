# MyRucio

My instructions for Rucio 

Reference:

    https://twiki.cern.ch/twiki/bin/view/CMSPublic/Rucio
    
Where:

    /afs/cern.ch/user/a/amassiro/work/Rucio
    
Commands to prepare:

    source /cvmfs/cms.cern.ch/cmsset_default.sh
    voms-proxy-init -voms cms -rfc -valid 192:00
    source /cvmfs/cms.cern.ch/rucio/setup.sh
    export RUCIO_ACCOUNT=`whoami` # Or your CERN username if it differs


Commands:

    rucio list-rules cms:/MiniDaq/Commissioning2020-v1/RAW

    
    
Get account:

    https://twiki.cern.ch/twiki/bin/view/CMSPublic/RucioUserDocsQuotas
    
    rucio list-rse-attributes T2_CH_CERN

See rules 

    rucio rule-info <id number>

    
    
