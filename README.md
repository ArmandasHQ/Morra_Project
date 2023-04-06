# The first "ONE"
goal app create --creator $ONE --approval-prog /data/build/approval.teal --clear-prog /data/build/clear.teal --global-byteslices 0 --global-ints 0 --local-byteslices 3 --local-ints 1
-------------------------------------------------------------
goal app optin --from $ONE --app-id 1

# The second "TWO"
goal app create --creator $TWO --approval-prog /data/build/approval.teal --clear-prog /data/build/clear.teal --global-byteslices 0 --global-ints 0 --local-byteslices 3 --local-ints 1
-------------------------------------------------------------
goal app optin --from $TWO --app-id 1


# if you are allready in /datadirctory
goal app create --approval-prog build/approval.teal --clear-prog build/clear.teal --global-byteslices 0 --global-ints 0 --local-byteslices 3 --local-ints 1 --creator $ONE