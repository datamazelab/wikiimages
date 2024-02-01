*******************************************************
*** Content Descriptions of the Supplemental Folder ***
*******************************************************

1. Description of main_experiment_data.csv
	- main_experiment_data.csv contains participant data collected through LabintheWild and Prolific platforms
	- this data contains the following fields:
		- praticipant_id: this id is a unique identifier for the participant
		- ed_level: taken from the demographics form, whose values can be: pre-high school, high school,
			    college, graduate school, professional school, postdoctoral, PhD
		- english: taken from the demographics form, can take one of the following values: beginner, 
			   basic, intermediate, upper-intermediate, and advanced
		- age: numeric value that participants reported as their age
		- platform: this field can be LabintheWild or Prolific, an indicator of which platform the participant
			    took the experiment from
		- img_pres: this field can be TRUE or FALSE, indicates if an image was displayed while participant viewed
			    associated article which can be identified using the "article_title" field. There was
			    a 50% chance for participants to see an image with their article.
		- q_type: this field can be non_vis, vis, and image. These are question types and are associated with the
			  the type of question participants answered for a given article, the exact question asked can be 
			  identified by looking at the "question" field. non_vis is associated with the general question type 
			  which means this question was generated to ask only about general features of the Wikipedia article,
			  like historic facts, or people identified with the given article topic. vis is associated with
			  visual question type generated to ask about the visual content of the Wikipedia article. image is
			  associated with visual question types, which indicates questions that asked participants to identify
			  an image that depicts the article topic they saw in their article.
		- indv_q_score: this field can be a 1 or 0. 1 indicates that the participant answered the associated "question"
				correctly, and a 0 indicates that they answered it incorrectly.
		- knowledge: (familiarity question) the answer to a five-nominal scale question on familiarity with the 
			     topic of the article. The scale categories were: 'I’ve never heard of it'(1), 'I’ve heard of it but 
			     I don’t know what it is'(2), 'I have some knowledge about this topic'(3), 'I know a lot about this
			     topic' (4), and 'I’m an expert on this topic'(5).
		- article_time: corresponds to the time taken by a participant to read or view an article
		- word_count: amount of words in the article participant saw
		- q_time: the difference between timestamps of when the participant first saw the question and when they 
			  clicked a blue arrow to see the next slide in the experiment
		- vis_q_consistency:  an indicator (only for visual questions) of whether the question could be answered 
    				      by looking at the image alone.
		- question: the question asked
		- article_title: title of the article participant saw before answering the question, can be used to find more
				 info on the article in articles.json or questions.csv
		- question_id: unique id used to identify the question, only relevant in this data set
		- article_id: unique article id used to identify the article, only relevant in this data set

2. Description of baseline_question_data.csv
	- baseline_question_data.csv was collected through Prolific platform
	- this data contains the following fields:
		- participant_id: this id is a unique identifier for the participant
		- ed_level: taken from the demographics form, whose values can be: pre-high school, high school,
			    college, graduate school, professional school, postdoctoral, PhD
		- english: taken from the demographics form, can take one of the following values: beginner, 
			   basic, intermediate, upper-intermediate, and advanced
		- age: numeric value that participants reported as their age
		- q_type:this field can be non_vis, vis, and image. These are question types and are associated with the
			  the type of question participants answered for a given article, the exact question asked can be 
			  identified by looking at the "question" field. non_vis is associated with the general question type 
			  which means this question was generated to ask only about general features of the Wikipedia article,
			  like historic facts, or people identified with the given article topic. vis is associated with
			  visual question type generated to ask about the visual content of the Wikipedia article. image is
			  associated with visual question types, which indicates questions that asked participants to identify
			  an image that depicts the article topic they saw in their article.
		- indv_q_score: this field can be a 1 or 0. 1 indicates that the participant answered the associated "question"
				correctly, and a 0 indicates that they answered it incorrectly.
		- knowledge: (familiarity question) the answer to a five-nominal scale question on familiarity with the 
			     topic of the article. The scale categories were: 'I’ve never heard of it'(1), 'I’ve heard of it but 
			     I don’t know what it is'(2), 'I have some knowledge about this topic'(3), 'I know a lot about this
			     topic' (4), and 'I’m an expert on this topic'(5).
		- q_time:the difference between timestamps of when the participant first saw the question and when they 
			  clicked a blue arrow to see the next slide in the experiment
		- vis_q_consistency:  an indicator (only for visual questions) of whether the question could be answered 
    				      by looking at the image alone.
		- question: the question asked
		- article_title: title of the article participant saw before answering the question, can be used to find more
				 info on the article in articles.json or questions.csv
		- article_id: unique article id used to identify the article, only relevant in this data set

3. Description of questions.csv
	- questions.csv is manually generated data
	- this data contains the following fields:
		- pageTitle: title of the article, taken from Wikipedia 
		- imageURL: url of the infobox image that was taken from the Wikipedia page directly
		- question1: 1 of 2 non-vis/general question types generated using the Wikipedia page
		- question2: 2 of 2 non-vis/general question types generated using the Wikipedia page
		- question3: 1 of 2 vis/visual question types generated using the Wikipedia page 
		- question4: 2 of 2 vis/visual question types generated using the Wikipedia page 
		- answer1: correct answer to question1
		- answer2: correct answer to question2
		- answer3: correct answer to question3
		- answer4: correct answer to question4
		- distractors1: distractors generated for question1
		- distractors2: distractors generated for question2
		- distractors3: distractors generated for question3
		- distractors4: distractors generated for question4
		- imageQuestion: image question generated for the article, usually of the format 
				 "Which is ..."
		- imageAnswerURL: url to the correct image answer for imageQuestion
		- imageDistracto1: 1 of 3 image question distractor answers
		- imageDistractor2: 2 of 3 image question distractor answers
		- imageDistractor3: 3 of 3 image question distractor answers

4. Description of articles.json
	- articles.json was manually generated and contains excerpts taken from Wikipedia articles that
	  were used to generate question in questions.csv
	- this data contains the following fields:
		- pageTitle: title of the Wikipedia article
		- sectionTitles: list of sub-sections for which excerpts were taken
		- (fields for each section title): contains the excerpt taken directly from Wikipedia

5. Description of AsPredicted_preregistration.pdf (AsPredicted (for peer-review only) #68156)
	- Pre-registered experiment document.

6. Description of Supplementary_Results.pdf
	- Supplemental results that include practice round question data as part of the entire analysis for the experiment and some visual examples.

7. Description of Additional_experimental_details.pdf
	- Supplemental experimental details including metrics definitions and participant demographics.
8. Flowcharts
	- directory containing textual flowcharts describing baseline and full experiment

