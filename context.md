Project Name: DESIboli : A Real-Time Auction System with Collaborative Buying

---

1. Project Overview

Create a Real-time auction system as a desktop website, primarily focusing on Indian handmade products like vases, sculptures, and paintings,etc . (Add more Indian handmade products on your own)

The system will have two types of auctions:

1. Normal Bidding: A single user can bid individually.
2. Collaborative Bidding: Users can form teams and bid together by pooling their money. The team with the highest bid wins.


Key Requirements:

- Website should have Smooth scroll animation/transitions on landing page (don't take too much burden on this,but put some).
- An aesthetic UI which is matching the given color palette.
- Real-time bidding updates via WebSockets (Socket.io).
- Payment integration via Razorpay.
- Admin panel for managing auctions.
- Step-by-step development approach to avoid overwhelming complexity.

---

2. Tech Stack

- Frontend: Next.js + Tailwind CSS
- Backend: Node.js + Express.js
- Database: MongoDB (Mongoose ORM)
- Real-Time Communication: Socket.io (WebSockets)
- Payment Integration: Razorpay

---

3. Pages & Features

3.1 Landing Page

- Website Name: DESIboli (use the best-looking font according to the theme).
- Brief description of the platform and its features.
- Visually appealing UI with the following:
- "Get Started" Button : Redirects to the Marketplace Page.
- Login/Signup Button : Optional for users (they can still participate without logging in).
- Hero Section : A high-quality banner with a brief about auctions and handmade products.
- Featured Auctions Section : Displays top ongoing auctions dynamically.
- Testimonials Section : Show some dummy user reviews to add credibility.
- Footer Section : Links to Contact Us, Privacy Policy, Terms & Conditions.

---

3.2 Marketplace Page

Displays all available auction items divided into two sections:

1. Normal Bidding
2. Collaborative Bidding

Users can view item details, including:

- Name
- Image
- Description
- Current Highest Bid (Auto-updated in real-time)
- Time Left for Auction End

Search & Filter Options:

- Users can filter items by category (paintings, vases, sculptures, etc.)
- Sort by Highest Bid / Lowest Bid / Newest Auctions

---

3.3 Normal Bidding (Single User Bidding)

- Any registered or guest user can place a bid on an auction item.
- The bid must be higher than the current highest bid.

Live bidding updates:
- If a new bid is placed, all users see the update in real-time.
- If a user's bid is outbid, they receive an instant notification.

Auction Countdown Timer:
- Each auction item shows a countdown timer until the auction ends.
- When time runs out, the highest bidder is declared the winner.

---

3.4 Collaborative Bidding (Team-Based Bidding)

- Users can form a team and pool their money to place a bid.
- Each team member contributes a portion of the total bid.
- Other teams can place higher bids in real-time.
- Once time expires, the team with the highest bid wins.

Team Formation Process:
1. A user creates a team and sets the minimum contribution amount.
2. Other users can join the team and contribute.
3. Once the team has enough funds, they can place a bid.
4. The team with the highest bid at the end of the auction wins.

---

3.5 Real-Time Bidding System (Essential Features)

- WebSockets (Socket.io) for Live Bidding Updates
- Instant notifications for outbids
- Auto-refresh bid history & current highest bid
- Live countdown timer for auction expiry
- Bid validation to prevent lower bids
- Dynamic leaderboards for highest bidders/teams

---

3.6 Auction Winner & Payment Processing

1. Auction End Logic:

- When the auction time ends, the highest bidder/team wins.
- The winning user/team gets a popup notification:
- "Congratulations! You won the auction. Please proceed to payment."

2. Payment via Razorpay:

- The winner is redirected to Razorpay for payment processing.
- Once payment is successful, they receive a "Payment Received" pop-up.

3. Item Ownership Transfer:

- After successful payment, the item is marked as sold.
- Other bidders receive a notification that the auction has ended.

---

3.7 Admin Panel (Auction Management)

- Admin Login (Basic authentication)
- Add/Edit/Delete auction items
- Set start & end times for auctions
- View bid history & auction analytics
- Manage users & transactions

---

4. Additional Features That a Real-Time Auction System Must Have :

1. Auction History Page:
Users can view past auctions, winners, and final price.

2. Transaction Management & Refunds:
- If a winner fails to pay within a deadline, the item goes to the second-highest bidder.
- Refund option for unsuccessful transactions.

---

5. Development Roadmap (Step-by-Step Approach)

Don't take too much burden , proceed with one step at a time(you can divide the task on your own also and complete one task at a time) and if you complete that part then ask me "should I proceed for next part ?"  And when I say yes "Continue with next part " then start with next part.
