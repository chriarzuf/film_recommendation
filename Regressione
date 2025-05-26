--Regressione

CREATE OR REPLACE MODEL
  `tmdb_dataset.user_rating_predictor_model`
OPTIONS
  (model_type='LINEAR_REG',
    input_label_cols=['label'],
    calculate_p_values = TRUE, -- Aggiungi QUESTA opzione
    CATEGORY_ENCODING_METHOD='DUMMY_ENCODING'
  )
AS
SELECT
  *
FROM
  `tmdb_dataset.user_film_ratings_training`;
