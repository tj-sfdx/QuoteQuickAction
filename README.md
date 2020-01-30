# QuoteQuickAction
This requires three items: 
* Opportunity Quick Action
* Flow
* Lightning Component

It works like this:
* The Quick Action calls the Flow
* The Flow looks up the record id of the opportunity then passes that information into the Ltgn Cmp.
* The Ltgn Cmp gathers the input from the user, creates the new Quote, then redirects the page to the quote line items

# Build the Lightning Component first
Code for this is in this repository.  (You can change the lightning:recordEditForm to a lightning:recordForm if you want to use a layout instead of having to specify each field individually)

# Build the flow
I dunno how to upload a flow here but essentially it should look like this:
* Screen flow
* Have a Variable with the name of recordId
* Lookup the Opp with the recordId, then pass that into the lightning component
*
