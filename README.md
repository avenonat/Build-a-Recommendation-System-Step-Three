# Build-a-Recommendation-System-Step-Three

For the last part of the capstone, you will integrate your recommender program with our course site. This will enable you to let a user run your program interactively on the internet.

Review criteria
less 
You will submit your project by copying and pasting the link to the web page that runs your recommender. Reviewers will look at your project to confirm that all the required parts are complete.

Basic Requirements Checklist

Does your program display a reasonable number of movies for the user to rate?
Does your program successfully recommend at least one movie to the user?
Does your program correctly display the results in an HTML table?For the last part of the capstone, you will integrate your recommender program with our course site. This will enable you to let a user run your program interactively on the internet.

Review criteria
less 
You will submit your project by copying and pasting the link to the web page that runs your recommender. Reviewers will look at your project to confirm that all the required parts are complete.

Basic Requirements Checklist

Does your program display a reasonable number of movies for the user to rate?
Does your program successfully recommend at least one movie to the user?
Does your program correctly display the results in an HTML table?
Instructions
less 
For the last part of the capstone, you will integrate your recommender program with our course site. This will enable you to let a user run your program interactively on the internet. The user will be presented with a list of movies to rate, they will submit their ratings, and then a list of movies recommended for them by your program will be displayed. You will be able to choose which movies the user is presented to rate, and how to display the recommended movies.

You will have to write a class that will allow the course site to run your recommender program, and then you will have to create a zip file of the code to be uploaded.

Write a Class

For this assignment you will be given one interface Recommender. You will have to write a class RecommendationRunner that implements Recommender. The two methods you will need to implement are:

getItemsToRate()
printRecommendationsFor()
When the user first visits the recommender site, our code will call the method getItemsToRate() to get a list of movies to display on the web page for users to rate. After the user submits their ratings, our code will call the method printRecommendationsFor() to get your recommendations based on the user's ratings and display them.

Specifically, you should:

Create a new class named RecommendationRunner that implements Recommender.
Write the method getItemsToRate(). It returns a list of strings representing movie IDs that will be used to present movies to the user for them to rate. You can choose how to select movies for this list, for example, you could select recent movies, movies from a specific genre, randomly chosen movies, or something else. The movies returned by this method will be displayed on a web page, so the number of movies you choose to return may affect how long the page takes to load, and how willing users will be to rate the movies. 10-20 movies should be fine to get a good profile of the user’s opinions, but 50 may be too many.
Write the void method printRecommendationsFor(). It prints out an HTML table of movies recommended by your program for the user based on the movies they rated. It has one parameter webRaterID, a String that is the ID of the user, who has been added by our code to the RaterDatabase with the ratings they entered. To get the movies recommended by your program, you may want to use your FourthRatings class. Because the HTML printed by this method will be displayed on a webpage, the number of recommended movies you choose to display may affect how long the page takes to load. For example, you may want to display only the top 10-20 recommended movies, or to not include movies the user rated. In some rare cases there may not be any recommended movies, for example, if no movies were rated by the number of minimal raters specified in the recommender. If no movies are recommended, you should notify the user with a message. Whatever is printed by this method will be displayed on the web page: HTML, plain text, or debugging information. If you want to style this HTML page, please include the CSS styling directly within the page using the <style> tag.
Instructions
less 
For the last part of the capstone, you will integrate your recommender program with our course site. This will enable you to let a user run your program interactively on the internet. The user will be presented with a list of movies to rate, they will submit their ratings, and then a list of movies recommended for them by your program will be displayed. You will be able to choose which movies the user is presented to rate, and how to display the recommended movies.

You will have to write a class that will allow the course site to run your recommender program, and then you will have to create a zip file of the code to be uploaded.

Write a Class

For this assignment you will be given one interface Recommender. You will have to write a class RecommendationRunner that implements Recommender. The two methods you will need to implement are:

getItemsToRate()
printRecommendationsFor()
When the user first visits the recommender site, our code will call the method getItemsToRate() to get a list of movies to display on the web page for users to rate. After the user submits their ratings, our code will call the method printRecommendationsFor() to get your recommendations based on the user's ratings and display them.

Specifically, you should:

Create a new class named RecommendationRunner that implements Recommender.
Write the method getItemsToRate(). It returns a list of strings representing movie IDs that will be used to present movies to the user for them to rate. You can choose how to select movies for this list, for example, you could select recent movies, movies from a specific genre, randomly chosen movies, or something else. The movies returned by this method will be displayed on a web page, so the number of movies you choose to return may affect how long the page takes to load, and how willing users will be to rate the movies. 10-20 movies should be fine to get a good profile of the user’s opinions, but 50 may be too many.
Write the void method printRecommendationsFor(). It prints out an HTML table of movies recommended by your program for the user based on the movies they rated. It has one parameter webRaterID, a String that is the ID of the user, who has been added by our code to the RaterDatabase with the ratings they entered. To get the movies recommended by your program, you may want to use your FourthRatings class. Because the HTML printed by this method will be displayed on a webpage, the number of recommended movies you choose to display may affect how long the page takes to load. For example, you may want to display only the top 10-20 recommended movies, or to not include movies the user rated. In some rare cases there may not be any recommended movies, for example, if no movies were rated by the number of minimal raters specified in the recommender. If no movies are recommended, you should notify the user with a message. Whatever is printed by this method will be displayed on the web page: HTML, plain text, or debugging information. If you want to style this HTML page, please include the CSS styling directly within the page using the <style> tag.
