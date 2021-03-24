# valence-control
Data, code, and tasks for Dorfman, et al., 2019, Psych Science.

Citation for use of any code, data, or task: 
Dorfman, H. M., Bhui, R., Hughes, B. L., & Gershman, S. J. (2019). Causal Inference About Good and Bad Outcomes. Psychological Science, 133, 956797619828724. http://doi.org/10.1177/0956797619828724

Tasks

The behavioral tasks used for both experiments in the paper are provided here. They were written using Josh deLeeuw's jsPsych toolbox (http://www.jspsych.org/).

Both tasks will not run "out of the box" because they require communication with a PHP server. You can achieve this by running them on your own domain, or by using a tool like XAMPP to run the PHP server locally. You could also use an easy-to-use experiment hosting service, my favorite of which is: https://www.cognition.run/. Please note that slight modifications may need to be made to the existing code to either run the task locally or on a hosting service. For example, the consent and data save functions will need to be commented out in order to run the task locally (if you do not have PHP capabilities). For more information on running online jsPsych experiments, please see the extensive documentation available on the jsPsych website, Github discussion forum, and particularly here: https://www.jspsych.org/overview/running-experiments/.

Data

The data for all of the participants included in both experiments are provided here. The variable names can be found in the headers of these csv files, and a key is provided below. The csvs provided have been minimally processed for ease of use specifically for model-fitting (i.e., single subject csvs have been concatenated, all output has been made numeric, and variables unnecessary for analyses have been removed).
Code for the model fitting can be found here and on the OSF. These analyses require the mfit package developed by Sam Gershman (https://github.com/sjgershm/mfit). Many of the plotting and modeling functions were also developed by Sam Gershman.

Variable Key

feedback: reward feedback received (0 = negative outcome, 1 = positive outcome)

latent_agent: did the latent agent intervene on this trial? (0 = no, 1 = yes)

subject: unique, non-identifiable subject ID number

latent_prob: probability of latent agent intervention for this version of the task

mine_prob_win_left: probability of a positive outcome for the stimulus on the left side

mine_prob_win_right: probability of a positive outcome for the stimulus on the right side

latent_guess: button press for subject guess about latent agent intervention (0 = no, agent did not intervene, 1 = yes, agent did intervene)

block_num: block order

trial_num: trial number

condition: condition (1 = adversarial, 2 = benvolent, or 3 = random)

subj_choice: button press (1 = left, 2 = right)

Contact

For questions, please contact Hayley Dorfman (hdorfman@g.harvard.edu).



