# tracking-demo
trackingtest:	demo database root

serials:		supposedly auto-generated values which will
		be individually attached to each eWagan 
		created

eWagans:		information about eWagans (i.e.
			birth (timestamp)
			status: {dead, alive}
				dead: not owned by a user
				alive: owned by a user

users:		info about registered users
			id
			name
			...

netWorth (refactored)	every entry is indexed by a userId, values under an ID
			are the eWagans the user owns

transactions	every transfer of wagan's from user to user is recorded
			serial
			timestamp
			fromUser
			toUser

In addition, we will be creating the web front end that will:
1.Allow registration and editing of User Profiles for the SMS APP Firebase.
2.Read and present transaction data from the SMS APP Firebase.
3.Perform web based transactions that will write to the SMS APP Firebase.
  a)This includes bulk transactions such as:
    i.Deduction of 3% eWagan from every User at a specific data and time every three months to be sent to the Guiuan Wagan account.
    ii.The selection of multiple Users to send Government/NGO payments. (Eg. Cash for Work distribution of 1000 eWagan to 500 Users from NGO Account)
4.Allow Users to track all Wagan & eWagan that they created.
5.Allow the public to view dynamic reports or download sanitized tracking data.
6.(Later, allow the online purchase and sending of eWagan.)
