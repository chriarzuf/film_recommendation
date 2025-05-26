--Training set creation

CREATE OR REPLACE TABLE
  `tmdb_dataset.user_film_ratings_training` AS
SELECT
  f.popularity,
  f.vote_average,
  f.War AS genre_War,
  f.Adventure AS genre_Adventure,
  f.Fantasy AS genre_Fantasy,
  f.Animation AS genre_Animation,
  f.Drama AS genre_Drama,
  f.TV_Movie AS genre_TV_Movie,
  f.Horror AS genre_Horror,
  f.Action AS genre_Action,
  f.Music AS genre_Music,
  f.Comedy AS genre_Comedy,
  f.History AS genre_History,
  f.Western AS genre_Western,
  f.Mistery AS genre_Mistery,
  f.Thriller AS genre_Thriller,
  f.Crime AS genre_Crime,
  f.Documentary AS genre_Documentary,
  f.Science_Fiction AS genre_Science_Fiction,
  f.Romance AS genre_Romance,
  f.Family AS genre_Family,
  r.Rating AS label -- La nostra variabile target
FROM
  `tmdb_dataset.film_extended` AS f
JOIN
  `tmdb_dataset.ratings-test` AS r
ON
  f.title = r.Name;
