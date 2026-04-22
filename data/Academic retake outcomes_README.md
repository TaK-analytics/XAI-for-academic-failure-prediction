# Academic retake outcomes
Educational profile data and digital footprint of university students who failed their exam session in the previous semester. The data covers 2 previous semesters and the current semester of study. 

### Variables:

| Feature | Type and Possible Values | Description |
|---------|--------------------------|-------------|
| code | string | Student ID<br>*Уникальный идентификатор студента* |
| ac_year | categorical<br>(1, 2)| Academic year<br>*Академический год* |
| year_of_study | integer<br>(1,2,..,6) | Year of study<br>*Текущий год обучения студента* |
| semester | binary<br>(1 - Fall, 2 - Spring) | Semester<br>*Семестр* |
| gender | categorical<br>(0 - Female, 1 - Male) | Student gender<br>*Пол студента* |
| age | float<br>\[0, 1\] | Student's age, mapped to \[0, 1\] using a monotonically increasing function<br>*Возраст студента, отображенный в \[0, 1\]  с помощью монотонно возрастающей функции*|
| int_status | categorical<br>(0 - local/1 - international)| Indicator of foreign citizenship or international enrollment<br>*Индикатор наличия иностранного гражданства или международного набора на программу*|
| faculty | categorical| Faculty (encoded)<br>*Факультет(закодирован)*|
| funding_type | categorical<br>(SF - state-funded, TP - tuition-paying, TT - targeted training ) |Funding type<br>*Тип финансирования*|
| program_level | categorical<br>(Bachelor, Specialist) | Degree level<br>*Уровень программы* |
| num_ac_leaves | integer | Total number of academic leaves taken since enrollment<br>*Количество академических отпусков с момента поступления*|
| num_trasfers | integer | Total number of transfers to other degree programs within the university since enrollment<br>*Количество переводов с другой программы в рамках университета* |
| num_dismissals | integer | Total number of prior academic dismissals from the university<br>*Количество предыдущих отчислений из университета* |
| num_courses_previous_sem | integer | Total number of courses enrolled in the previous semester<br>*Количество учебных дисциплин в предыдущем семестре* |
| num_pass/fail_exams_previous_sem | integer | Total number of pass/fail exams in the previous semester<br>*Количество зачетов в предыдущем семестре* |
| num_graded_exams_previous_sem | integer | Total number of graded exams in the previous semester<br>*Количество экзаменов  в предыдущем семестре* |
| GPA_previous_sem | float | GPA in the immediately preceding semester, before retakes<br>*Средний балл зачетной книжки за предыдущий семестр до пересдач* |
| num_debts_graded_exams_previous_sem | integer | Total number of failed graded exams from previous semester (not yet retaken)<br>*Количество долгов по экзаменам с оценкой за предыдущий семестр (которые еще не пересданы)* |
| num_debts_pass/fail_exams_previous_sem | integer | Total number of failed pass/fail exams from previous semester (not yet retaken)<br>*Количество долгов по зачётам за предыдущий семестр (которые еще не пересданы)*|
| GPA_after_first_retakes_previous_sem | float  | GPA in the previous semester after including results of first retakes<br>*Средний балл зачетной книжки после первой пересдачи за предыдущий семестр* |
| num_debts_graded_exams_<br>after_first_retakes_previous_sem | integer | Number of failed graded exams from previous semester (after first retakes passed)<br>*Количество долгов по экзаменам за предыдущий семестр после первой пересдачи* |
| num_debts_pass/fail_exams_<br>after_first_retakes_previous_sem | integer | Number of failed pass/fail exams from previous semester (after first retakes passed)<br>*Количество долгов по зачётам за предыдущий семестр после первой пересдачи*  |
| GPA_after_second_retakes_previous_sem | float  | GPA in the previous semester after including results of second retakes<br>*Средний балл зачетки после второй пересдачи за предыдущий семестр* |
| num_debts_graded_exams_<br>after_second_retakes_previous_sem | integer | Number of failed graded exams from previous semester (after second retakes passed)<br>*Количество долгов по экзаменам предыдущего семестра после второй пересдачи*|
| num_debts_pass/fail_exams_<br>after_second_retakes_previous_sem | integer | Number of failed pass/fail exams from previous semester (after second retakes passed)<br>*Количество долгов по зачётам предыдущего семестра после второй пересдачи*|
| num_courses_2sem_prior | integer | Number of courses enrolled from two semesters prior<br>*Количество учебных дисциплин за 2 семестра до текущего* |
| num_pass/fail_exams_2sem_prior | integer | Total number of pass/fail exams from two semesters prior<br>*Количество зачётов за 2 семестра до текущего* |
| num_graded_exams_2sem_prior | integer |  Total number of graded exams from two semesters prior<br>*Количество экзаменов с оценкой за 2 семестра до текущего* |
| GPA_2sem_prior | float| GPA in the semester before the previous one, before retakes<br>*Средний балл зачетной книжки за 2 семестра до текущего* |
| num_debts_graded_exams_2sem_prior | integer | Number of failed graded exams from two semesters prior (not yet retaken)<br>*Количество долгов по экзаменам, полученных за 2 семестра до текущего и еще не пересданных* |
| num_debts_pass/fail_exams_2sem_prior | integer | Number of failed pass/fail exams from two semesters prior (not yet retaken)<br>*Количество долгов по зачётам, полученных за 2 семестра до текущего и еще не пересданных* |
| GPA_after_first_retakes_2sem_prior | float | GPA from two se-mesters prior after including results of first retakes<br>*Средний балл зачетной книжки за два семестра до текущего после первой пересдачи* |
| num_debts_graded_exams_<br>after_first_retakes_2sem_prior | integer | Number of failed graded exams from two semesters prior (after first retakes passed)<br>*Число долгов за экзамены сессии за 2 семестра до текущего после первой пересдачи* |
| num_debts_pass/fail_exams_<br>after_first_retakes_2sem_prior | integer | <Number of failed pass/fail exams from two semesters prior (after first retakes passed)<br>*Число долгов за зачеты сессии за 2 семестра до текущего после первой пересдачи* |
| prop_debts_previous_sem | float (0.0..1.0) |The ratio of the number of failed courses to the total number of courses in the previous semester before retakes<br>*Отношение числа несданных дисциплин в общему числу дисциплин в прошлов семестре до проведения пересдач*|
| prop_debts_after_first_retakes_previous_sem | float (0.0..1.0) | The ratio of the number of failed courses to the total number of courses in the previous semester after first retakes<br>*Отношение числа несданных дисциплин в общему числу дисциплин в прошлос семестре после периода первых пересдач*|
| prop_debts_2sem_prior | float (0.0..1.0) | The ratio of the number of failed courses to the total number of courses in the semester (from 2 semesters prior)<br>*Отношение числа несданных дисциплин в общему числу дисциплин в семестре за 2 семестра до текущего до проведения пересдач*|
| prop_debts_after_first_retakes_2sem_prior | float (0.0..1.0) | The ratio of the number of failed courses to the total number of courses in the semester (from 2 semesters prior) afer first retakes<br>*Отношение числа несданных дисциплин в общему числу дисциплин в семестре за 2 семестра до текущего после периода первых пересдач*|
|**for N = 3, 4, 7, 10, 17, 18:**|||
| active_clicks_week_N | float| Total count of user interactions with the LMS by week N of the current semester (standardized by dividing by the average number of active clicks in their study group)<br>*Количество кликов в LMS к неделе N текущего семестра (стандартизованное делением на среднее число кликов в учебной группе)*|
| effective_clicks_week_N | float| Total count of effective\* user interactions with the LMS by week N of the current semester (standardized by dividing by the average number of effective clicks in their study group)<br>*Количество эффективных\* кликов в LMS к неделе N текущего семестра (стандартизованное делением на среднее число эффективных кликов в учебной группе)*|
| score_week_N | float| Average grade across all e-courses the student is enrolled in by the week N of the current semester (standardized by dividing by the average score in their study group)<br>*Средний балл студента по всем электронным курсам, к которым он подписан в LMS, к неделе N текущего семестра (стандартизованное делением на среднее значение этого показателя в учебной группе)*|
| downtime_week_N | integer | Total duration of inactivity in the LMS (in weeks) by week N of the current semester<br>*Длительность отсутствия активности студента в LMS (в неделях) к неделе N текущего семестра*|
| active_clicks_week_N_previous_sem | float|Total count of user interactions with the LMS by week N of the previous semester (standardized)<br>*Количество кликов в LMS к неделе N предыдущего семестра (стандартизованное)*|
| effective_clicks_week_N_previous_sem | float | Total count of effective user interactions with the LMS by week N of the previous semester (standardized)<br>*Количество эффективных кликов в LMS к неделе N предыдущего семестра (стандартизованное)* |
| score_week_N_previous_sem | float | Average grade across all e-courses the student is enrolled in by the week N of the previous semester (standardized)<br>*Средний балл студента по всем электронным курсам, к которым он подписан в LMS, к неделе N предыдущего семестра (стандартизованное)*|
| downtime_week_N_previous_sem | integer | Total duration of inactivity in the LMS (in weeks) by week N of the previous semester<br>*Длительность отсутствия активности студента в LMS (в неделях) к неделе N предыдущего семестра*|
| active_clicks_week_N_2sem_prior | float|Total count of user interactions with the LMS by week N two semesters prior (standardized)<br>*Количество кликов в LMS к неделе N два семестра назад (стандартизованное) |
| effective_clicks_week_3_2sem_prior |  float | Total count of effective user interactions with the LMS by week N two semesters prior (standardized)<br>*Количество эффективных кликов в LMS к неделе N два семестра назад (стандартизованное)*  |
| score_week_3_2sem_prior | float |Average grade across all e-courses the student is enrolled in by the week N two semesters prior (standardized)<br>*Средний балл студента по всем электронным курсам, к которым он подписан в LMS, к неделе N два семестра назад (стандартизованное)* |
| downtime_week_3_2sem_prior | integer | Total duration of inactivity in the LMS (in weeks) by week N two semesters prior<br>*Длительность отсутствия активности студента в LMS (в неделях) к неделе N два семестра назад* |

\* **Effective clicks** — interactions with the e-course that change its content, e.g., submitting assignments, test attempts, etc. 

\* **Эффективные клики** — *взаимодействя пользователя с электронным курсом, которое меняет его содержимое, например, отправка на проверку выполненных заданий, прохождение попытки тестирования и т.п.* 
