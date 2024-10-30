# nosql-challenge
Challenge 12 - by Olga Petrova

## Eat Safe, Love magazine food safety ratings.

I explored 39780 restaurants and cafes in UK with hygiene score 0 to 20 to see how many pass health and safety code.
The goal was to find establishments with score 0 (did not pass health and safety) to see how many of them in each city.

There is a new restaurant Penang Flavours opened in London. The task was to see how many 0 - 5 score restaurants are near by it.
### Question 1: Which establishments have a hygiene score equal to 20? 
There are 41 establishments with a hygiene score equal to 20.
These are the first 10:
```
	BusinessName	Hygiene
0	TIWA N TIWA African Restaurant Ltd	5
1	Iceland	0
2	Howe and Co Fish and Chips - Van 17	0
3	Volunteer	0
4	Atlantic Fish Bar	0
5	Lumbini Grocery Ltd T/A Al-Iman	0
6	Plumstead Manor Nursery	0
7	Greggs	0
8	Tesco	0
9	Dosa & Sambal Express	0
```

### Question 2: Which establishments in London have a RatingValue greater than or equal to 4?
There are 33 establishments with a RatingValue greater than or equal to 4. 
These are the first 10:
```
_id	BusinessName	RatingValue
0	67214d24924c1b64ee59ecc8	Charlie's	4
1	67214d24924c1b64ee59efee	Mv City Cruises Erasmus	5
2	67214d24924c1b64ee59fb3f	Benfleet Motor Yacht Club	4
3	67214d24924c1b64ee5a0939	Tilbury Seafarers Centre	5
4	67214d24924c1b64ee5a093a	Coombs Catering t/a The Lock and Key	5
5	67214d24924c1b64ee5a1042	Mv Valulla	5
6	67214d25924c1b64ee5a3153	Tereza Joanne	5
7	67214d25924c1b64ee5a3519	Brick Lane Brews	4
8	67214d25924c1b64ee5a3533	The Nuance Group (UK) Limited	5
9	67214d25924c1b64ee5a3534	WH Smith	5
```

### Question 3: What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
Here are 10 of them within degree_search 0.01:
```
	_id	BusinessName	Hygiene	longitude	latitude
0	67214d25924c1b64ee5a2b0c	Volunteer	0	0.092080	51.487344
1	67214d25924c1b64ee5a2b22	Atlantic Fish Bar	0	0.091216	51.486730
2	67214d25924c1b64ee5a2b26	Lumbini Grocery Ltd T/A Al-Iman	0	0.091626	51.487163
3	67214d25924c1b64ee5a2ae0	Iceland	0	0.092420	51.487148
4	67214d25924c1b64ee5a2aee	Howe and Co Fish and Chips - Van 17	0	0.092537	51.487534
```

### Question 4: How many establishments in each Local Authority area have a hygiene score of 0?
There are 55 establishments with hygiene score 0 in these locations:
```
_id	count
0	Thanet	1130
1	Greenwich	882
2	Maidstone	713
3	Newham	711
4	Swale	686
5	Chelmsford	680
6	Medway	672
7	Bexley	607
8	Southend-On-Sea	586
9	Tendring	542
```
