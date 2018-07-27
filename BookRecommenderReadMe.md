# Book-Crossing Recommender System

This project seeks to create a book recommendation model from the [Book-Crossing](http://www.bookcrossing.com/) dataset ([available here](http://www2.informatik.uni-freiburg.de/~cziegler/BX/)).

## Resources
Building a recommendation system: [full workflow](https://towardsdatascience.com/building-a-recommendation-system-for-fragrance-5b00de3829da) - github repo [here](https://github.com/kellypeng/scentmate_rec).

Implementing recommender sys [from scratch in Python](https://cambridgespark.com/content/tutorials/implementing-your-own-recommender-systems-in-Python/index.html).

---------------------------------------------------
## Dataset Format
The Book-Crossing dataset is comprised of 3 tables:

1. BX-Users   
This contains the Book-Crossing users. There is a 'User-ID', and some demographic data ('Location', 'Age') if available.

2. BX-Books  
Books are identified by their ISBN number, and invalid ISBNs have already been removed from the dataset. Where available, book information is given here ('Book-Title', 'Book-Author', 'Year-Of-Publication', 'Publisher'). If there are several authors for one book, only the first is given. URLs linking to cover images are also given in small, medium, and large formats ('Image-URL-S', 'Image-URL-M', 'Image-URL-M').

3. BX-Book-Ratings  
Contains all of the book rating info. Ratings ('Book-Rating') are either EXPLICIT (on a scale of 1-10 - higher being better), or IMPLICIT, which is expressed by a 0. i.e. a ZERO is NOT a bad rating, but just an *implicit* one.

---------------------------------------------------
## Data Download
The datasets were downloaded as a csv dump, where the first line contains column names and fields are separated by a semi-colon.



