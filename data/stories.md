## story_01_location
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_01_location_02
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_01_location_03
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart


## story_01_location_not
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots

## story_01_location_02_not
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots

## story_01_location_03_not
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots


## story_02_location
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_02_location_01
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_02_location_02
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_03_location_deny
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "valid"}  
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart


## story_03_location_01_deny
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}  
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart


## story_03_location_02_deny
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart



## story_03_location
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "valid"}  
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_03_location_01
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}  
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_03_location_02
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart



## story_05_location
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_05_location_01
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_05_location_02
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
* action_search_restaurants{"cuisine": "Chinese"}
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart



## story_06_location
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}  
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}  
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* deny
  - utter_did_that_help
* affirm
  - utter_happy
  - utter_bye
  - action_restart


## story_08_location
* greet
  - utter_greet
* action_search_restaurants
  - utter_ask_location
* out_of_scope
  - action_slot_reset
  - utter_location_invalid
  - utter_ask_location_retry
* deny
  - utter_deny
  - utter_bye
  - action_restart

## story_09_location
* greet
  - utter_greet
* action_search_restaurants{"location": "Mumbai", "cuisine": "chinese"}
  - action_location_valid
  - action_cuisine_valid
  - slot{"location_validity" : "invalid"}  
  - utter_location_invalid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_location_retry
* affirm
  - utter_ask_location
* action_search_restaurants{"location": "Mumbai"}
  - utter_ask_budget
* ask_budget{"price": "high"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_10_location
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Mumbai"}
    - slot{"location": "Mumbai"}
    - action_location_valid
    - slot{"location_validity": "valid"}
    - utter_ask_cuisine
* cuisine{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - utter_ask_budget
* price{"price": "mid"}
    - slot{"price": "mid"}
    - action_search_restaurants
    - slot{"location": "Mumbai"}
    - slot{"search_validity": "valid"}
    - utter_ask_details
* not
    - utter_bye
    - action_slot_reset
    - reset_slots

## story_11_location
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Chandigarh"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Chandigarh"}
    - action_location_valid
    - slot{"location_validity": "valid"}
    - utter_ask_budget
* price{"price": "mid"}
    - slot{"price": "mid"}
    - action_search_restaurants
    - slot{"location": "Chandigarh"}
    - slot{"search_validity": "valid"}
    - utter_ask_details
* not
    - utter_bye
    - action_slot_reset
    - reset_slots

## story_12_location
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Chandigarh"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Chandigarh"}
    - action_location_valid
    - utter_location_invalid
    - slot{"cuisine_validity" : "valid"}
    - utter_ask_location_retry
* affirm
  - utter_ask_location
* price{"price": "mid"}
    - slot{"price": "mid"}
    - action_search_restaurants
    - slot{"location": "Chandigarh"}
    - slot{"search_validity": "valid"}
    - utter_ask_details
* not
    - utter_bye
    - action_slot_reset
    - reset_slots

## story_02_location
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_02_location_01
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart

## story_02_location_02
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "invalid"}
* deny
  - utter_deny
  - utter_bye
  - action_slot_reset  
  - action_restart


## story_01_location
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_01_location_02
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart

## story_01_location_03
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* ask_email{"email": "abc@abc.com"}
  - action_send_email
  - utter_confirm_email
* thank
  - utter_bye
  - action_restart


## story_01_location_not
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "invalid"}
  - utter_location_invalid
  - utter_ask_location_retry
* affirm
  - utter_ask_location  
  - action_slot_reset
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots

## story_01_location_02_not
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "invalid"}
  - utter_cuisine_invalid
  - utter_ask_cuisine_retry
* affirm
  - utter_ask_cuisine
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots

## story_01_location_03_not
* greet
  - utter_greet
* action_search_restaurants{"location": "Bangalore"}
  - action_location_valid
  - slot{"location_validity" : "valid"}
  - utter_ask_cuisine  
* action_search_restaurants{"cuisine": "Chinese"}
  - action_cuisine_valid
  - slot{"cuisine_validity" : "valid"}
  - utter_ask_budget
* ask_budget{"price": "low"}
  - action_search_restaurants
  - slot{"search_validity" : "valid"}
  - utter_ask_details
* affirm
  - utter_ask_email
* not
  - utter_bye
  - action_slot_reset
  - reset_slots