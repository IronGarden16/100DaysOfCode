## Day 0: Re-do
I'm going to Re-do my 100 days of code challenge. I've been so busy in the last few 
because of school and personal related things. I've thought of making a medium blog, but
it seems like long posts aren't my thing. Maybe this kind of micro blogging works out for me.

## Day 1: I've already started
I already have an on-going project that I'll be personally using on a day to day basis.
Its the web-based expense tracking app. The plan is after I finished the front-end, I'll
move my data from firebase to other free hosting such as heroku.

I've already added the table for transactions. Although its not much, it should be fine for
starters. And so today I added a couple of formatting, refactoring, and transaction form and dialog.

## Day 2: Still a long way to go
I've only coded for less than an hour today. Although I've only coded for a short time, I've learned
an important lesson (for me at least) that I should always put the mutations and actions to the
methods section of a vue component. I refactored the form of the transaction to use the store for its
data model.

## Day 3: Transaction complete
I added the firestore integration for the addition of transaction. I used 
`firestore.firebase.Timestamp.fromDate(new Date())` to get the current time and date for my
transaction dates since Firebase doesn't have their own `NOW()` equivalent from SQL aside from the said 
technique.

## Day 4: Google, Who is this?
Today, I added a way to login. Currently, I'm only using google's firebase auth and will
add new ways to login if I see it fit. I refactored the `route.js` to have its own directory since
I'll have new files like `routeRules.js` that is related to the routes. Refactor routes so that
they'll use names defined on a constants file. Refactor store so that they're in a directory and
add constants file.

## Day 5: Refactor
Today I refactored the store to be on their own module. I also namespaced them. I might remove
the namespacing since I believe it introduced more layers of the store than wanted eg. rootGetters etc.
I removed the type column on the transaction table and add the type indication via text color and
additional indication via text (+ and -).