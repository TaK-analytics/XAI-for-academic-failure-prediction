# Academic retake outcomes
Educational profile data and digital footprint of university students who failed their exam session in the previous semester. The data covers 2 previous semesters and the current semester of study. 

### Variables:

| Feature | Type and Possible Values | Description |
|---------|--------------------------|-------------|
| code | string | Student ID<br>Уникальный идентификатор студента |
| ac_year | categorical<br>(1, 2)| Academic year<br>Академический год |
| year_of_study | integer<br>(1,2,..,6) | Year of study<br>Текущий год обучения студента |
| semester | binary<br>(1 - Fall, 2 - Spring) | Semester<br>Семестр |
| gender | categorical<br>(0 - Female, 1 - Male) | Student gender<br>Пол студента |
| age | numerical<br>\[0, 1\] | Student's age, mapped to \[0, 1\] using a monotonically increasing function<br>Возраст студента, отображенный в \[0, 1\]  с помощью монотонно возрастающей функции|
| int_status | categorical<br>(0 - local/1 - international)| International Status<br>Статус интернациональности (local/international) |
| faculty | categorical (string) | Название факультета |
| funding_type | categorical | Тип финансирования (бюджет/контракт) |
| program_level | categorical | Уровень программы (бакалавр/магистр и т.д.) |
| num_ac_leaves | integer (0..N) | Количество академических отпусков |
| num_trasfers | integer (0..N) | Количество переводов с другой программы/курса |
| num_dismissals | integer (0..N) | Количество отчислений (восстановлений) |
| num_courses_previous_sem | integer | Количество курсов в предыдущем семестре |
| num_pass/fail_exams_previous_sem | integer | Количество экзаменов типа зачёт/незачёт в предыдущем семестре |
| num_graded_exams_previous_sem | integer | Количество экзаменов с оценкой в предыдущем семестре |
| GPA_previous_sem | float (0.0..5.0) | Средний балл (GPA) за предыдущий семестр |
| num_debts_graded_exams_previous_sem | integer | Количество долгов по экзаменам с оценкой за предыдущий семестр |
| num_debts_pass/fail_exams_previous_sem | integer | Количество долгов по зачётным экзаменам за предыдущий семестр |
| GPA_after_first_retakes_previous_sem | float (0.0..5.0) | GPA после первой пересдачи за предыдущий семестр |
| num_debts_graded_exams_<br>after_first_retakes_previous_sem | integer | Количество долгов по оценкам после первой пересдачи (пред. семестр) |
| num_debts_pass/fail_exams_<br>after_first_retakes_previous_sem | integer | Количество долгов по зачётам после первой пересдачи (пред. семестр) |
| GPA_after_second_retakes_previous_sem | float (0.0..5.0) | GPA после второй пересдачи за предыдущий семестр |
| num_debts_graded_exams_<br>after_second_retakes_previous_sem | integer | Количество долгов по оценкам после второй пересдачи (пред. семестр) |
| num_debts_pass/fail_exams_<br>after_second_retakes_previous_sem | integer | Количество долгов по зачётам после второй пересдачи (пред. семестр) |
| num_courses_2sem_prior | integer | Количество курсов за 2 семестра до текущего |
| num_pass/fail_exams_2sem_prior | integer | Количество зачётных экзаменов за 2 семестра до текущего |
| num_graded_exams_2sem_prior | integer | Количество экзаменов с оценкой за 2 семестра до текущего |
| GPA_2sem_prior | float (0.0..5.0) | GPA за 2 семестра до текущего |
| num_debts_graded_exams_2sem_prior | integer | Количество долгов по оценкам (2 семестра назад) |
| num_debts_pass/fail_exams_2sem_prior | integer | Количество долгов по зачётам (2 семестра назад) |
| GPA_after_first_retakes_2sem_prior | float (0.0..5.0) | GPA после первой пересдачи (2 семестра назад) |
| num_debts_graded_exams_<br>after_first_retakes_2sem_prior | integer | Долги по оценкам после первой пересдачи (2 сем. назад) |
| num_debts_pass/fail_exams_<br>after_first_retakes_2sem_prior | integer | Долги по зачётам после первой пересдачи (2 сем. назад) |
| prop_debts_previous_sem | float (0.0..1.0) | Доля долгов за предыдущий семестр (до пересдач) |
| prop_debts_after_first_retakes_previous_sem | float (0.0..1.0) | Доля долгов после первой пересдачи (пред. семестр) |
| prop_debts_2sem_prior | float (0.0..1.0) | Доля долгов за 2 семестра до текущего |
| prop_debts_after_first_retakes_2sem_prior | float (0.0..1.0) | Доля долгов после первой пересдачи (2 сем. назад) |
| active_clicks_week_3 | integer (0..N) | Количество активных кликов на 3-й неделе |
| effective_clicks_week_3 | integer (0..N) | Количество эффективных кликов на 3-й неделе |
| score_week_3 | float (0..100) | Балл активности на 3-й неделе |
| downtime_week_3 | float (часы) | Время простоя (бездействия) на 3-й неделе |
| active_clicks_week_3_previous_sem | integer | Активные клики на 3-й неделе предыдущего семестра |
| effective_clicks_week_3_previous_sem | integer | Эффективные клики на 3-й неделе предыдущего семестра |
| score_week_3_previous_sem | float | Балл на 3-й неделе предыдущего семестра |
| downtime_week_3_previous_sem | float | Время простоя на 3-й неделе предыдущего семестра |
| active_clicks_week_3_2sem_prior | integer | Активные клики на 3-й неделе (2 семестра назад) |
| effective_clicks_week_3_2sem_prior | integer | Эффективные клики на 3-й неделе (2 семестра назад) |
| score_week_3_2sem_prior | float | Балл на 3-й неделе (2 семестра назад) |
| downtime_week_3_2sem_prior | float | Время простоя на 3-й неделе (2 семестра назад) |
| active_clicks_week_4 | integer | Активные клики на 4-й неделе |
| effective_clicks_week_4 | integer | Эффективные клики на 4-й неделе |
| score_week_4 | float | Балл на 4-й неделе |
| downtime_week_4 | float | Время простоя на 4-й неделе |
| active_clicks_week_4_previous_sem | integer | Активные клики на 4-й неделе предыдущего семестра |
| effective_clicks_week_4_previous_sem | integer | Эффективные клики на 4-й неделе предыдущего семестра |
| score_week_4_previous_sem | float | Балл на 4-й неделе предыдущего семестра |
| downtime_week_4_previous_sem | float | Время простоя на 4-й неделе предыдущего семестра |
| active_clicks_week_4_2sem_prior | integer | Активные клики на 4-й неделе (2 семестра назад) |
| effective_clicks_week_4_2sem_prior | integer | Эффективные клики на 4-й неделе (2 семестра назад) |
| score_week_4_2sem_prior | float | Балл на 4-й неделе (2 семестра назад) |
| downtime_week_4_2sem_prior | float | Время простоя на 4-й неделе (2 семестра назад) |
| active_clicks_week_7 | integer | Активные клики на 7-й неделе |
| effective_clicks_week_7 | integer | Эффективные клики на 7-й неделе |
| score_week_7 | float | Балл на 7-й неделе |
| downtime_week_7 | float | Время простоя на 7-й неделе |
| active_clicks_week_7_previous_sem | integer | Активные клики на 7-й неделе предыдущего семестра |
| effective_clicks_week_7_previous_sem | integer | Эффективные клики на 7-й неделе предыдущего семестра |
| score_week_7_previous_sem | float | Балл на 7-й неделе предыдущего семестра |
| downtime_week_7_previous_sem | float | Время простоя на 7-й неделе предыдущего семестра |
| active_clicks_week_7_2sem_prior | integer | Активные клики на 7-й неделе (2 семестра назад) |
| effective_clicks_week_7_2sem_prior | integer | Эффективные клики на 7-й неделе (2 семестра назад) |
| score_week_7_2sem_prior | float | Балл на 7-й неделе (2 семестра назад) |
| downtime_sem2_week_7 | float | Время простоя на 7-й неделе 2-го семестра (спец. метрика) |
| active_clicks_week_10 | integer | Активные клики на 10-й неделе |
| effective_clicks_week_10 | integer | Эффективные клики на 10-й неделе |
| score_week_10 | float | Балл на 10-й неделе |
| downtime_week_10 | float | Время простоя на 10-й неделе |
| active_clicks_week_10_previous_sem | integer | Активные клики на 10-й неделе предыдущего семестра |
| effective_clicks_week_10_previous_sem | integer | Эффективные клики на 10-й неделе предыдущего семестра |
| score_week_10_previous_sem | float | Балл на 10-й неделе предыдущего семестра |
| downtime_week_10_previous_sem | float | Время простоя на 10-й неделе предыдущего семестра |
| active_clicks_week_10_2sem_prior | integer | Активные клики на 10-й неделе (2 семестра назад) |
| effective_clicks_week_10_2sem_prior | integer | Эффективные клики на 10-й неделе (2 семестра назад) |
| score_week_10_2sem_prior | float | Балл на 10-й неделе (2 семестра назад) |
| downtime_week_10_2sem_prior | float | Время простоя на 10-й неделе (2 семестра назад) |
| active_clicks_week_17 | integer | Активные клики на 17-й неделе |
| effective_clicks_week_17 | integer | Эффективные клики на 17-й неделе |
| score_week_17 | float | Балл на 17-й неделе |
| downtime_week_17 | float | Время простоя на 17-й неделе |
| active_clicks_week_17_previous_sem | integer | Активные клики на 17-й неделе предыдущего семестра |
| effective_clicks_week_17_previous_sem | integer | Эффективные клики на 17-й неделе предыдущего семестра |
| score_week_17_previous_sem | float | Балл на 17-й неделе предыдущего семестра |
| downtime_week_17_previous_sem | float | Время простоя на 17-й неделе предыдущего семестра |
| active_clicks_week_17_2sem_prior | integer | Активные клики на 17-й неделе (2 семестра назад) |
| effective_clicks_week_17_2sem_prior | integer | Эффективные клики на 17-й неделе (2 семестра назад) |
| score_week_17_2sem_prior | float | Балл на 17-й неделе (2 семестра назад) |
| downtime_sem2_week_17 | float | Время простоя на 17-й неделе 2-го семестра |
| active_clicks_week_18 | integer | Активные клики на 18-й неделе |
| effective_clicks_week_18 | integer | Эффективные клики на 18-й неделе |
| score_week_18 | float | Балл на 18-й неделе |
| downtime_week_18 | float | Время простоя на 18-й неделе |
| active_clicks_week_18_previous_sem | integer | Активные клики на 18-й неделе предыдущего семестра |
| effective_clicks_week_18_previous_sem | integer | Эффективные клики на 18-й неделе предыдущего семестра |
| score_week_18_previous_sem | float | Балл на 18-й неделе предыдущего семестра |
| downtime_week_18_previous_sem | float | Время простоя на 18-й неделе предыдущего семестра |
| active_clicks_week_18_2sem_prior | integer | Активные клики на 18-й неделе (2 семестра назад) |
| effective_clicks_week_18_2sem_prior | integer | Эффективные клики на 18-й неделе (2 семестра назад) |
| score_week_18_2sem_prior | float | Балл на 18-й неделе (2 семестра назад) |
