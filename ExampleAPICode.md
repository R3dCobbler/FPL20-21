# Example Code used in the FPL API.
Showing endpoints used to compile each of the tables to be included in the WDC

## Main end point  ("https://fantasy.premierleague.com/api/bootstrap-static/"). Note that this is the new URL for the API. (Old one was "https://fantasy.premierleague.com/drf/bootstrap-static/". Just replace 'drf' with 'api')

This contains the following types of information

### Events Information   (Shows Gameweek info)

"events": [{
	"id":1,
	"name":"Gameweek 1",
	"deadline_time":"2020-09-12T12:30:00Z",
	"average_entry_score":0,
	"finished":false,
	"data_checked":false,
	"highest_scoring_entry":null,
	"deadline_time_epoch":1599913800,
	"deadline_time_game_offset":0,
	"highest_score":null,
	"is_previous":false,
	"is_current":false,
	"is_next":true,
	"chip_plays":[],
	"most_selected":null,
	"most_transferred_in":null,
	"top_element":null,
	"top_element_info":null,
	"transfers_made":0,
	"most_captained":null,
	"most_vice_captained":null}, 

### Game Settings Information

"game_settings":{
	"league_join_private_max":25,
	"league_join_public_max":5,
	"league_max_size_public_classic":20,
	"league_max_size_public_h2h":16,
	"league_max_size_private_h2h":16,
	"league_max_ko_rounds_private_h2h":3,
	"league_prefix_public":"League",
	"league_points_h2h_win":3,
	"league_points_h2h_lose":0,
	"league_points_h2h_draw":1,
	"league_ko_first_instead_of_random":false,
	"cup_start_event_id":17,
	"cup_stop_event_id":38,
	"cup_qualifying_method":"event",
	"cup_type":"random",
	"squad_squadplay":11,
	"squad_squadsize":15,
	"squad_team_limit":3,
	"squad_total_spend":1000,
	"ui_currency_multiplier":10,
	"ui_use_special_shirts":false,
	"ui_special_shirt_exclusions":[],
	"stats_form_days":30,
	"sys_vice_captain_enabled":true,
	"transfers_sell_on_fee":0.5,
	"league_h2h_tiebreak_stats":["+goals_scored","-goals_conceded"],
	"timezone":"UTC"
	},

### Phases Information  (Shows Month start and end gameweeks)

"phases": [{
		"id": 1,
		"name": "Overall",
		"start_event": 1,
		"stop_event": 38
	}, 


### Team Information   

"teams":[{
	"code":3,
	"draw":0,
	"form":null,
	"id":1,
	"loss":0,
	"name":"Arsenal",
	"played":0,
	"points":0,
	"position":0,
	"short_name":"ARS",
	"strength":null,
	"team_division":null,
	"unavailable":false,
	"win":0,
	"strength_overall_home":0,
	"strength_overall_away":0,
	"strength_attack_home":0,
	"strength_attack_away":0,
	"strength_defence_home":0,
	"strength_defence_away":0,
	"pulse_id":1
	}, 

### Total FPL Players
"total_players":458715,


### Player Information   (Be aware of some minor differences to the old api)

"elements":[{
	"chance_of_playing_next_round":null,
	"chance_of_playing_this_round":null,
	"code":37605,
	"cost_change_event":0,
	"cost_change_event_fall":0,
	"cost_change_start":0,
	"cost_change_start_fall":0,
	"dreamteam_count":0,
	"element_type":3,
	"ep_next":"0.0",
	"ep_this":null,
	"event_points":0,
	"first_name":"Mesut",
	"form":"0.0",
	"id":1,
	"in_dreamteam":false,
	"news":"",
	"news_added":null,
	"now_cost":70,
	"photo":"37605.jpg",
	"points_per_game":"0.0",
	"second_name":"Özil",
	"selected_by_percent":"2.6",
	"special":false,
	"squad_number":null,
	"status":"a",
	"team":1,
	"team_code":3,
	"total_points":53,
	"transfers_in":0,
	"transfers_in_event":0,
	"transfers_out":0,
	"transfers_out_event":0,
	"value_form":"0.0",
	"value_season":"7.6",
	"web_name":"Özil",
	"minutes":1439,
	"goals_scored":1,
	"assists":3,
	"clean_sheets":5,
	"goals_conceded":20,
	"own_goals":0,
	"penalties_saved":0,
	"penalties_missed":0,
	"yellow_cards":1,
	"red_cards":0,
	"saves":0,
	"bonus":1,
	"bps":256,
	"influence":"223.6",
	"creativity":"582.9",
	"threat":"190.0",
	"ict_index":"99.8",
	"influence_rank":251,
	"influence_rank_type":108,
	"creativity_rank":35,
	"creativity_rank_type":29,
	"threat_rank":174,
	"threat_rank_type":95,
	"ict_index_rank":135,
	"ict_index_rank_type":72
	}, 

### Player Stats Information

"element_stats":[{
	"label":"Minutes played",
	"name":"minutes"
	}, {
	"label":"Goals scored",
	"name":"goals_scored"
	}, {
	"label":"Assists",
	"name":"assists"
	}, {
	"label":"Clean sheets",
	"name":"clean_sheets"
	}, {
	"label":"Goals conceded",
	"name":"goals_conceded"
	}, {
	"label":"Own goals",
	"name":"own_goals"
	}, {
	"label":"Penalties saved",
	"name":"penalties_saved"
	}, {
	"label":"Penalties missed",
	"name":"penalties_missed"
	}, {
	"label":"Yellow cards",
	"name":"yellow_cards"
	}, {
	"label":"Red cards",
	"name":"red_cards"
	}, {
	"label":"Saves",
	"name":"saves"
	}, {
	"label":"Bonus",
	"name":"bonus"
	}, {
	"label":"Bonus Points System",
	"name":"bps"
	}, {
	"label":"Influence",
	"name":"influence"
	}, {
	"label":"Creativity",
	"name":"creativity"
	}, {
	"label":"Threat",
	"name":"threat"
	}, {
	"label":"ICT Index",
	"name":"ict_index"
}],

### Player Type Information

"element_types":[{
	"id":1,
	"plural_name":"Goalkeepers",
	"plural_name_short":"GKP",
	"singular_name":"Goalkeeper",
	"singular_name_short":"GKP",
	"squad_select":2,
	"squad_min_play":1,
	"squad_max_play":1,
	"ui_shirt_specific":true,
	"sub_positions_locked":[12],
	"element_count":47
	},

## Fixture Information   ("https://fantasy.premierleague.com/api/fixtures/") 
 
### For a game already played (Example from the 1st game of Gameweek 1: Liverpool 4 Norwich 1)
[{
	"code": 1059702,
	"event": 1,
	"finished": true,
	"finished_provisional": true,
	"id": 1,
	"kickoff_time": "2019-08-09T19:00:00Z",
	"minutes": 90,
	"provisional_start_time": false,
	"started": true,
	"team_a": 14,
	"team_a_score": 1,
	"team_h": 10,
	"team_h_score": 4,
	"stats": [{
		"identifier": "goals_scored",
		"a": [{
			"value": 1,
			"element": 278  
		}],
		"h": [{
			"value": 1,
			"element": 183
		}, {
			"value": 1,
			"element": 188
		}, {
			"value": 1,
			"element": 191
		}]
	}, {
		"identifier": "assists",
		"a": [{
			"value": 1,
			"element": 283
		}],
		"h": [{
			"value": 1,
			"element": 182
		}, {
			"value": 1,
			"element": 187
		}, {
			"value": 1,
			"element": 188
		}, {
			"value": 1,
			"element": 191
		}]
	}, {
		"identifier": "own_goals",
		"a": [{
			"value": 1,
			"element": 277
		}],
		"h": []
	}, {
		"identifier": "penalties_saved",
		"a": [],
		"h": []
	}, {
		"identifier": "penalties_missed",
		"a": [],
		"h": []
	}, {
		"identifier": "yellow_cards",
		"a": [{
			"value": 1,
			"element": 283
		}, {
			"value": 1,
			"element": 288
		}],
		"h": []
	}, {
		"identifier": "red_cards",
		"a": [],
		"h": []
	}, {
		"identifier": "saves",
		"a": [{
			"value": 4,
			"element": 280
		}],
		"h": [{
			"value": 2,
			"element": 189
		}, {
			"value": 2,
			"element": 526
		}]
	}, {
		"identifier": "bonus",
		"a": [{
			"value": 1,
			"element": 278
		}],
		"h": [{
			"value": 3,
			"element": 188
		}, {
			"value": 2,
			"element": 191
		}]
	}, {
		"identifier": "bps",
		"a": [{
			"value": 32,
			"element": 278
		}, {
			"value": 19,
			"element": 280
		}, {
			"value": 18,
			"element": 273
		}, {
			"value": 16,
			"element": 274
		}, {
			"value": 16,
			"element": 283
		}, {
			"value": 15,
			"element": 276
		}, {
			"value": 12,
			"element": 286
		}, {
			"value": 11,
			"element": 290
		}, {
			"value": 10,
			"element": 287
		}, {
			"value": 3,
			"element": 434
		}, {
			"value": 2,
			"element": 277
		}, {
			"value": 1,
			"element": 285
		}, {
			"value": -3,
			"element": 288
		}],
		"h": [{
			"value": 46,
			"element": 188
		}, {
			"value": 40,
			"element": 191
		}, {
			"value": 27,
			"element": 183
		}, {
			"value": 26,
			"element": 187
		}, {
			"value": 24,
			"element": 182
		}, {
			"value": 18,
			"element": 197
		}, {
			"value": 15,
			"element": 181
		}, {
			"value": 12,
			"element": 198
		}, {
			"value": 11,
			"element": 199
		}, {
			"value": 10,
			"element": 184
		}, {
			"value": 7,
			"element": 189
		}, {
			"value": 7,
			"element": 526
		}, {
			"value": 3,
			"element": 192
		}, {
			"value": 3,
			"element": 200
		}]
	}],
	"team_h_difficulty": 2,
	"team_a_difficulty": 5
}, 

### For a game yet to be played
{
	"code": 1060081,
	"event": 38,
	"finished": false,
	"finished_provisional": false,
	"id": 380,
	"kickoff_time": "2020-05-17T14:00:00Z",
	"minutes": 0,
	"provisional_start_time": false,
	"started": false,
	"team_a": 2,
	"team_a_score": null,
	"team_h": 19,
	"team_h_score": null,
	"stats": [],
	"team_h_difficulty": 2,
	"team_a_difficulty": 3
}]

## Player History Information  ("https://fantasy.premierleague.com/api/element-summary/176/")
Example data for element #176 

### Forthcoming Fixture Information

"fixtures": [{
		"code": 1059767,
		"team_h": 9,
		"team_h_score": null,
		"team_a": 13,
		"team_a_score": null,
		"event": 7,
		"finished": false,
		"minutes": 0,
		"provisional_start_time": false,
		"kickoff_time": "2019-09-29T15:30:00Z",
		"event_name": "Gameweek 7",
		"is_home": true,
		"difficulty": 2
	}, 

### Current Season Information 

"history": [{
		"element": 176,
		"fixture": 5,
		"opponent_team": 20,
		"total_points": 3,
		"was_home": true,
		"kickoff_time": "2019-08-11T13:00:00Z",
		"team_h_score": 0,
		"team_a_score": 0,
		"round": 1,
		"minutes": 90,
		"goals_scored": 0,
		"assists": 0,
		"clean_sheets": 1,
		"goals_conceded": 0,
		"own_goals": 0,
		"penalties_saved": 0,
		"penalties_missed": 0,
		"yellow_cards": 0,
		"red_cards": 0,
		"saves": 0,
		"bonus": 0,
		"bps": 15,
		"influence": "20.2",
		"creativity": "13.8",
		"threat": "3.0",
		"ict_index": "3.7",
		"value": 50,
		"transfers_balance": 0,
		"selected": 69367,
		"transfers_in": 0,
		"transfers_out": 0
	}, 


### Past History Information  
Data from Season 2016-17, 2017-18, 2018-19, 2019-20

"history_past": [
    {
      "season_name": "2011/12",
      "element_code": 82514,
      "start_cost": 40,
      "end_cost": 40,
      "total_points": 22,
      "minutes": 1170,
      "goals_scored": 0,
      "assists": 1,
      "clean_sheets": 0,
      "goals_conceded": 26,
      "own_goals": 0,
      "penalties_saved": 0,
      "penalties_missed": 0,
      "yellow_cards": 1,
      "red_cards": 0,
      "saves": 0,
      "bonus": 4,
      "bps": 0,
      "influence": "0.0",
      "creativity": "0.0",
      "threat": "0.0",
      "ict_index": "0.0"
    },
    {
      "season_name": "2018/19",
      "element_code": 82514,
      "start_cost": 45,
      "end_cost": 42,
      "total_points": 50,
      "minutes": 2046,
      "goals_scored": 0,
      "assists": 0,
      "clean_sheets": 5,
      "goals_conceded": 49,
      "own_goals": 0,
      "penalties_saved": 0,
      "penalties_missed": 0,
      "yellow_cards": 1,
      "red_cards": 0,
      "saves": 0,
      "bonus": 4,
      "bps": 349,
      "influence": "331.6",
      "creativity": "46.3",
      "threat": "3.0",
      "ict_index": "38.3"
    }
  ]
