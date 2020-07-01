# Snack Shack Requirements Specification

Hello, the competitive world of software engineering has gotten to me and I have decided to enter the world of
fast food!

I am making quick snacks but I would like a program to help organise people's orders and what I should be
doing.

As my business grows, I will most definately need to add features to the program.  I don't want to get ahead of myself though
so please complete each step in its entirety before moving on.

NOTE: The output should act like a schedule by displaying the time at which things would happen,
it should not act like a timer and wait for that duration.  E.g. The output for the first 
requirement one should display all the times at once, not take 6 minutes to run.

NOTE: While not required, it would be nice to see your solution after each requirement by way of a git repository
with a commit, tag or branch after each completed requirement.

## Requirement 1: Sandwiches

I can make a sandwich in one minute and then I need 30 seconds to serve the sandwich and take money from
the customer.

Can you write a program that takes orders from customers and sequences what I should be doing?

So if I have four sandwich orders the schedule should be:

1. 0:00 4 sandwich orders placed, start making sandwich 1
2. 1:00 serve sandwich 1
3. 1:30 make sandwich 2
4. 2:30 serve sandwich 2
5. 3:00 make sandwich 3
6. 4:00 serve sandwich 3
7. 4:30 make sandwich 4
8. 5:30 serve sandwich 4
9. 6:00 take a well earned break!

## Requirement 2: Estimates

With the schedule in place I should be able to predict when people will get their order when they place it.

Modify your program so that when an order is placed it returns an estimate of how long the customer will have
to wait from the order being placed to getting their food, based on the current order.
Fast food, short tempers

People expect to be able to get their sandwich quickly. If they have to wait more than five minutes they will
refuse to pay for it. So in the example above sandwich 4 would have been too late.
Modify the order placement so that it rejects orders that cannot be served in time.

## Requirement 3: Inventory

I only have limited ingredients in the shack: I can only make 45 sandwiches. Orders for something that is sold
out should not be accepted. Add inventory tracking to the program and reject orders that cannot be fulfilled.

## Requirement 4: Jacket potatoes

Sandwiches are great but people really want the option of hot food too. I've decided to offer jacket potatoes.
Jacket potatoes are pre-baked but need to be heated in a microwave for 2 and half minutes. I then need 30
seconds to top them and 30 seconds to serve them.

Jacket potatoes go cold again if they are not served within two minutes of being heated.

The good news is that people will wait seven minutes to get a jacket potato.

Please modify the order system to include jacket potatoes.

So if there are orders for two sandwiches and a jacket potato the schedule should be:

1. 0:00 Put jacket potato in microwave
2. 0:01 Make sandwich 1
3. 1:01 Serve sandwich 1
4. 1:31 Make sandwich 2
5. 2:31 Serve sandwich 2
6. 3:01 take jacket potato out of microwave
7. 3:31 top jacket potato
8. 4:01 serve jacket potato
9. 4:31 take a break!

## Requirement 5: Potato inventory

I have enough stock to serve 30 jacket potatoes. Modify the program so that I it rejects orders for an item that
is sold out. However it should now offer an alternative if it is available, so if I order a sandwich and they are
sold out then I should see a list of alternatives that lists a jacket potato.

## Requirement 6: More microwaves, more potatoes?

If I buy more microwaves then I can cook more potatoes simultaneously. Modify the program so that I
configure how many microwaves I have. The program should warn me if I try to start more jacket potatoes
than I can finish and serve.
