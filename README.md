# Massive Data Project

Diabetes Mellitus (DM) is a metabolic impairment characterized by the inability to normally stabilize glucose blood levels; this impairment is conditioned by several causes, some of them are still unknown. 3 most common causes are:

Insulin resistance
Insulin secretion impairment
Glucose overproduction

There are 3 main types of diabetes, Type 1 (DM1), characterized by the early onset due to the autoimmune composition of it and by the need of external insulin injection, Type 2 (DM2), characterized by the increased resistance to insulin and by the close relationship with obesity and finally, Gestational Diabetes (DMG), characterized by the appearance during pregnancy.

Diabetes Mellitus has an increasing prevalence in nowadays society. In 1980 there were 109 millions of diabetics but in 2017 world hospitals dealt with 425 millions of diabetics. This disease is mainly present in the USA and in Europe and it has been on the WHO’s radar for a long time. Among all possible associated complications related to the disease, diabetic retinopathy, diabetic foot syndrome, angiopathies, cardiopathies and diabetic coma are the most present. These long-term complications appear due to bad management of the disease, being recurrently in a hypoglycemic or hyperglycemic state, slowly damaging all circulatory system-related organs, tissues and structures. That’s why it is crucial to detect diabetes as soon as possible. In this project diabetes hospital management will be evaluated in a 10 years frame for some USA hospitals trying to assess which factors are the most important for the correct diagnosis, recovery and long-term diabetes management. Databases used will be yielded by the Center for Clinical and Translational Research and the UCI Machine Learning Repository, with 100.000 instances and 55 attributes associated, it would be a Big Data-type medical analysis.

By a brief review to the state of art on this topic it is clear that the main path to assess diabetes is the Glucose Serum Test Result, this would be the result of glucose presence on blood at the arrival moment of the patient to the hospital. Precisely on the database used this feature would be a three class variable (“normal”, “>200” and “>300”) in which milligrams of glucose per blood deciliter (mg/dL) would be the measurement unit.

In this case of study, Glucose Serum Test Result would be coupled with several other features of the dataset trying to extract some valuable information for clinicians, patients and future researchers.
Since early screening and diagnosis is related with Glucose Serum Test Result (with high glucose values for those who enter to the hospital in a more critical state and medium-high glucose values for those early diagnosed) it seems like it would be a good start point to correlate it with:

Hospitalization time 
{Time in hospital}

Relapse possibilities, re-hospitalization and readmission time 
{Readmitted}

Number of previous hospitalary interventions prior to diabetes diagnosis 
{Number of outpatient visits}
{Number of emergency visits}
{Number of inpatient visits}

Primary vs Secondary diagnosis 
{Diagnosis 1}
{Diagnosis 2}
{Diagnosis 3}
{Number of diagnoses}

Admission type (emergency, urgent, elective, newborn..etc) 
{Admission type}

In this project there are several paths in order to clarify inefficiencies in prognosis, diagnosis, hospitalization, recovery and long-term management of diabetes. First one consists of the early detection of diabetes, for this purpose there will be an evaluation of all the visits to the hospital prior to the diagnosis in order to assess if they were diabetes related, so that there were possibilities of detecting the disease earlier than it finally was. Number of diagnosis and differences between 1st and 2nd diagnosis will be evaluated in order to detect if there is sufficiently strong evidence on recurrent failed diagnosis. It would be interesting to take attention to the admission type of all patients who seem to have received an initial failed diagnosis, in order to see if those patients enter the hospital in a more critical condition. Second path will consist of the assessment of the hospital. The focus on this part will be directed to hospitalization time and readmission time after the release of the patient.It would be crucial to connect that first part of the data inference with the second one, evaluating if it is related bad diagnosis, and entry conditions of the hospital due to the late detection of diabetes with the hospitalization time and relapse possibilities. As stated above the guiding thread of all this would be the Glucose Serum Test Result since it is a good marker for measuring if diagnosis was made early or late and it is also a good marker for how difficult the recovery would be. For prolonged in time values higher than 300 mg/dL the body will fall in a cetoacidosis state that would damage the patient internally. Depending on that exposure time to cetoacidosis, the patient could enter in a diabetic coma. For this project, following diabetes state of art, glucose values >300 mg/dL on the Glucose Serum Test will be considered as highly critical values. These values will be contrasted with hemoglobin A1c values that measure long term blood glucose changes. The test detects glucose proportion on hemoglobin, computing it as a mean and showing results as a measure for blood glucose presence for 1 month ago. This way, using these 2 measures, it is possible to see long and short term conditions of the patient when he/she enters the hospital.



Impact of HbA1c Measurement on Hospital Readmission Rates Database is composed of over 100000 patients all characterized by 50 features. In order to get a more centralized study only the directly correlated features were choosed,discarding features with missing values majority, leading with the following shown in figure 
