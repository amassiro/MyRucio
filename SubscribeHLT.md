As from 16th July 2021 joint meeting:

    account=xxxxxxxxxx
    activity=”Express"
    lifetime=$((86400 * 90)) # lifetime in seconds.
    comment=”HLT tests” #optional
    block=”cms:/Cosmics/Commissioning2021-v1/RAW#b02aa1c4-1b74-4a36-9eee-a7268a4dbcf9”
    copies=1
    rse_expression=“T2_CH_CERN”
    rucio add-rule --account $account --lifetime $lifetime --activity $activiy --comment $comment $block $copies $rse_expression


To find out the block a particular file belongs to, the following procedure can be used:

    file=/store/data/Commissioning2021/Cosmics/RAW/v1/000/342/728/00000/9fc6c6d1-c018-459b-bd64-e0ed3b7ac859.root
    rucio list-parent-dids cms:$file

