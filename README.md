# Global Health Observatory (GHO)

source: [data query api from WHO](http://apps.who.int/gho/data/node.resources.api?lang=en)

the file `etl/all_indicators.csv` contians all available indicators from the API.

the file `etl/all_countries.csv` contains all abailable countries from the API.

## files with malformed csv format

When we update the source files, remember to check these files.

* NCD_CCS_CRDPlan.csv
* NCD_CCS_CancerPlan.csv
* NCD_CCS_DiabPlan.csv
* NCD_CCS_CRDPlan.csv
* HRH_20.csv
* HRH_27.csv
* DEVICES12.csv 
* DEVICES21.csv 
* DEVICES22.csv
* WHS9_CBR.csv
* PerctestedANC.csv
* PercposANC.csv
* PercposSW.csv
* PercposMSM.csv
* PerctreatedANC.csv


## some indicators use a range of year in the year column

example: the datapoint for mdg_0000000013. the year column shows a range of years.

they are imported as it is for now, we may need to change this later.


## some of indicators are not measure type

for now all indicator concepts are measure, which is wrong. should fix that.


## below indicators are not time series

so they are not included in DDF

* m_survey_title_adult
* m_svy_national_adult
* m_svy_age_adult
* m_def_1_text_adult
* m_def_1_prev_adult
* m_def_2_text_adult
* m_def_2_prev_adult
* m_smkless_survey_title_adult
* m_smkless_svy_national_adult
* m_smkless_age_range_adult
* m_smkless_def_text_adult
* m_smkless_prev_adult
* m_survey_title_youth
* m_svy_national_youth
* m_svy_age_youth
* m_def_1_text_youth
* m_def_1_prev_youth
* m_def_2_text_youth
* m_def_2_prev_youth
* m_smkless_survey_title_youth
* m_smkless_svy_national_youth
* m_smkless_age_range_youth
* m_smkless_def_text_youth
* m_smkless_prev_youth
* camp_nat
* camp_gov_prog
* camp_mat_tested
* camp_aud_research
* camp_tv_radio
* camp_media_planning
* camp_news
* camp_airtime
* camp_eval_impact
* rev_type
* rev_year
* rev_curr
* rev_excise
* rev_vat
* rev_imp_other
* rev_govt_total
* r_excise_type
* r_excise_uniform_varied
* r_excise_specific_reliance
* r_excise_min_specific
* r_excise_retail_price_base
* r_afford_less
* r_afford_tax_auto_adjust
* r_admin_tax_stamps
* r_admin_duty_free_limited
* r_admin_duty_free_allowance
* r_excise_proportion
* r_afford_gdp
* r_afford_price_dispersion



