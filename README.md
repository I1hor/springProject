# Cinema API
## Functional Requirements for Cinema API
### 1. User Authentication and Authorization:

+ Users can register, login, and logout.
+ Admin users have elevated privileges to manage theaters, movies, and showtimes.
### 2. Theater Management:

+ Admin can create, update, and delete theaters.
+ Each theater has a name, location, and number of seats.
### 3. Movie Management:

+ Admin can add, update, and delete movies.
+ Each movie has a title, description, duration, and genre.
### 4. Showtime Management:

+ Admin can create, update, and delete showtimes.
+ Each showtime is associated with a specific movie and theater, and has a start time and end time.
### 5. Seat Reservation:

+ Users can see available seats for a specific showtime.
+ Users can reserve seats, and once reserved, those seats become unavailable for that showtime.
### 6. Ticketing:

+ Users can purchase tickets for reserved seats.
+ Tickets contain information about the showtime, seat numbers, and price.
### 7. Search and Filtering:

+ Users can search for movies by title or genre.
+ Users can filter movies by genre or duration.
### 8. Reviews and Ratings:

+ Users can view and submit reviews and ratings for movies.
+ Each review consists of a rating (1-5 stars) and optional comments.
### 9. Notifications:

+ Users receive notifications for successful reservations and ticket purchases.
+ Users receive reminders for upcoming showtimes.
### 10. Analytics and Reporting:

+ Admin can view analytics such as ticket sales, popular movies, and revenue.
+ Admin can generate reports on movie attendance and user activity.

## System Behaviors

### User Management:

+ Authentication (register, login, logout).
+ Authorization (admin vs regular user access).
### Theater and Movie Management:

+ CRUD operations for theaters and movies.
+ Associate movies with theaters.
### Showtime Management:

+ CRUD operations for showtimes.
+ Associate showtimes with movies and theaters.
### Seat Reservation:

+ Check seat availability.
+ Reserve seats for a specific showtime.
### Ticketing:

+ Purchase tickets.
+ View ticket details.
### Search and Filtering:

+ Search movies by title or genre.
+ Filter movies by genre or duration.
### Reviews and Ratings:

+ View movie reviews and ratings.
+ Submit reviews and ratings.
### Notifications:

+ Send notifications for reservations, ticket purchases, and reminders.
### Analytics and Reporting:

+ View analytics on ticket sales, popular movies, revenue.
+ Generate reports on movie attendance and user activity.

## REST API Endpoints:
### Authentication:

<br> POST /api/auth/register
<br> POST /api/auth/login
<br> POST /api/auth/logout
### Theater Management:

<br> GET /api/theaters
<br> GET /api/theaters/{theater_id}
<br> POST /api/theaters
<br> PUT /api/theaters/{theater_id}
<br> DELETE /api/theaters/{theater_id}
### Movie Management:

<br> GET /api/movies
<br> GET /api/movies/{movie_id}
<br> POST /api/movies
<br> PUT /api/movies/{movie_id}
<br> DELETE /api/movies/{movie_id}
### Showtime Management:

<br> GET /api/showtimes
<br> GET /api/showtimes/{showtime_id}
<br> POST /api/showtimes
<br> PUT /api/showtimes/{showtime_id}
<br> DELETE /api/showtimes/{showtime_id}
### Seat Reservation:

<br> GET /api/showtimes/{showtime_id}/seats
<br> POST /api/showtimes/{showtime_id}/seats/reserve
### Ticketing:

<br> POST /api/tickets/purchase
<br> GET /api/tickets/{ticket_id}
### Reviews and Ratings:

<br> GET /api/movies/{movie_id}/reviews
<br> POST /api/movies/{movie_id}/reviews
<br> GET /api/movies/{movie_id}/ratings
<br> POST /api/movies/{movie_id}/ratings
### Search and Filtering:


<br> GET /api/movies/search
<br> GET /api/movies/filter
### Notifications:

Notifications are typically handled via email or push notifications and might not have dedicated API endpoints.
### Analytics and Reporting:

Reports and analytics are often generated through background jobs or scheduled tasks, not always directly exposed via API.
