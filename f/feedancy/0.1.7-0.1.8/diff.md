# Comparing `tmp/feedancy-0.1.7.tar.gz` & `tmp/feedancy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.1.7.tar", max compression
+gzip compressed data, was "feedancy-0.1.8.tar", max compression
```

## Comparing `feedancy-0.1.7.tar` & `feedancy-0.1.8.tar`

### file list

```diff
@@ -1,139 +1,129 @@
--rw-r--r--   0        0        0      615 2023-08-03 08:27:58.705997 feedancy-0.1.7/README.md
--rw-r--r--   0        0        0      126 2023-08-03 08:27:58.677561 feedancy-0.1.7/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:27:58.399400 feedancy-0.1.7/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:27:58.399553 feedancy-0.1.7/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-08-03 08:27:58.407437 feedancy-0.1.7/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      896 2023-08-03 08:27:58.432544 feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-08-03 08:27:58.434608 feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      853 2023-08-03 08:27:58.431593 feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      908 2023-08-03 08:27:58.433265 feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-08-03 08:27:58.434038 feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      863 2023-08-03 08:27:58.436145 feedancy-0.1.7/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-08-03 08:27:58.438478 feedancy-0.1.7/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      830 2023-08-03 08:27:58.435248 feedancy-0.1.7/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      885 2023-08-03 08:27:58.436957 feedancy-0.1.7/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      917 2023-08-03 08:27:58.437810 feedancy-0.1.7/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0     1258 2023-08-03 08:27:58.441021 feedancy-0.1.7/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-08-03 08:27:58.446164 feedancy-0.1.7/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0     1222 2023-08-03 08:27:58.439435 feedancy-0.1.7/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0     1277 2023-08-03 08:27:58.442252 feedancy-0.1.7/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0     1312 2023-08-03 08:27:58.445116 feedancy-0.1.7/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      899 2023-08-03 08:27:58.447843 feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-08-03 08:27:58.450547 feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      859 2023-08-03 08:27:58.446992 feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-08-03 08:27:58.448712 feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-08-03 08:27:58.449781 feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      935 2023-08-03 08:27:58.453510 feedancy-0.1.7/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-08-03 08:27:58.460008 feedancy-0.1.7/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      899 2023-08-03 08:27:58.451500 feedancy-0.1.7/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      954 2023-08-03 08:27:58.455136 feedancy-0.1.7/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-08-03 08:27:58.457020 feedancy-0.1.7/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      876 2023-08-03 08:27:58.463108 feedancy-0.1.7/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-08-03 08:27:58.467585 feedancy-0.1.7/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      840 2023-08-03 08:27:58.461482 feedancy-0.1.7/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      895 2023-08-03 08:27:58.464625 feedancy-0.1.7/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      930 2023-08-03 08:27:58.466250 feedancy-0.1.7/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      881 2023-08-03 08:27:58.470793 feedancy-0.1.7/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-08-03 08:27:58.475319 feedancy-0.1.7/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      844 2023-08-03 08:27:58.469007 feedancy-0.1.7/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      899 2023-08-03 08:27:58.472334 feedancy-0.1.7/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      935 2023-08-03 08:27:58.473914 feedancy-0.1.7/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0     1922 2023-08-03 08:27:58.483594 feedancy-0.1.7/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-08-03 08:27:58.527059 feedancy-0.1.7/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0     1883 2023-08-03 08:27:58.477587 feedancy-0.1.7/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-08-03 08:27:58.486186 feedancy-0.1.7/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-08-03 08:27:58.503356 feedancy-0.1.7/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      917 2023-08-03 08:27:58.538388 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-08-03 08:27:58.550262 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      874 2023-08-03 08:27:58.533789 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      929 2023-08-03 08:27:58.540786 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-08-03 08:27:58.542777 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      935 2023-08-03 08:27:58.553108 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-08-03 08:27:58.556618 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      889 2023-08-03 08:27:58.551557 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      944 2023-08-03 08:27:58.554342 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-08-03 08:27:58.555714 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      923 2023-08-03 08:27:58.561857 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-08-03 08:27:58.569303 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      879 2023-08-03 08:27:58.558538 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      934 2023-08-03 08:27:58.564954 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      977 2023-08-03 08:27:58.567470 feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0     1627 2023-08-03 08:27:58.577415 feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-08-03 08:27:58.584249 feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0     1590 2023-08-03 08:27:58.572676 feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0     1645 2023-08-03 08:27:58.579401 feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1681 2023-08-03 08:27:58.583106 feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      874 2023-08-03 08:27:58.595176 feedancy-0.1.7/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-08-03 08:27:58.600067 feedancy-0.1.7/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      839 2023-08-03 08:27:58.591558 feedancy-0.1.7/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      894 2023-08-03 08:27:58.597952 feedancy-0.1.7/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      928 2023-08-03 08:27:58.599225 feedancy-0.1.7/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      969 2023-08-03 08:27:58.604845 feedancy-0.1.7/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-08-03 08:27:58.608643 feedancy-0.1.7/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      953 2023-08-03 08:27:58.602830 feedancy-0.1.7/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0     1008 2023-08-03 08:27:58.606095 feedancy-0.1.7/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0     1023 2023-08-03 08:27:58.607733 feedancy-0.1.7/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      966 2023-08-03 08:27:58.610965 feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-08-03 08:27:58.614705 feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      916 2023-08-03 08:27:58.609723 feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      971 2023-08-03 08:27:58.612177 feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1020 2023-08-03 08:27:58.613689 feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      896 2023-08-03 08:27:58.618144 feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-08-03 08:27:58.620377 feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      890 2023-08-03 08:27:58.617154 feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      945 2023-08-03 08:27:58.618908 feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-08-03 08:27:58.619783 feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      851 2023-08-03 08:27:58.622277 feedancy-0.1.7/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-08-03 08:27:58.624587 feedancy-0.1.7/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      817 2023-08-03 08:27:58.621132 feedancy-0.1.7/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      872 2023-08-03 08:27:58.623103 feedancy-0.1.7/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      905 2023-08-03 08:27:58.623963 feedancy-0.1.7/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      856 2023-08-03 08:27:58.626130 feedancy-0.1.7/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-08-03 08:27:58.628702 feedancy-0.1.7/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      821 2023-08-03 08:27:58.625316 feedancy-0.1.7/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      876 2023-08-03 08:27:58.627091 feedancy-0.1.7/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      910 2023-08-03 08:27:58.628048 feedancy-0.1.7/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      886 2023-08-03 08:27:58.630141 feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-08-03 08:27:58.632928 feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      845 2023-08-03 08:27:58.629429 feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      900 2023-08-03 08:27:58.631130 feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      940 2023-08-03 08:27:58.632055 feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2393 2023-08-03 08:27:58.640610 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2477 2023-08-03 08:27:58.653563 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3525 2023-08-03 08:27:58.635319 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2474 2023-08-03 08:27:58.643669 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2447 2023-08-03 08:27:58.650611 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      899 2023-08-03 08:27:58.656166 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-08-03 08:27:58.660022 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      859 2023-08-03 08:27:58.654865 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-08-03 08:27:58.657467 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-08-03 08:27:58.659001 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0     1039 2023-08-03 08:27:58.663205 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-08-03 08:27:58.668085 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      996 2023-08-03 08:27:58.661238 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0     1051 2023-08-03 08:27:58.664956 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0     1093 2023-08-03 08:27:58.667095 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      905 2023-08-03 08:27:58.670636 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-08-03 08:27:58.674883 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      864 2023-08-03 08:27:58.669248 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      919 2023-08-03 08:27:58.672034 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      959 2023-08-03 08:27:58.673812 feedancy-0.1.7/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-08-03 08:27:58.685011 feedancy-0.1.7/feedancy/client.py
--rw-r--r--   0        0        0        0 2023-08-03 08:27:58.690301 feedancy-0.1.7/feedancy/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:27:58.698401 feedancy-0.1.7/feedancy/lib/adapter/__init__.py
--rw-r--r--   0        0        0     2818 2023-08-03 08:27:58.696991 feedancy-0.1.7/feedancy/lib/adapter/aiohttp.py
--rw-r--r--   0        0        0      235 2023-08-03 08:27:58.701142 feedancy-0.1.7/feedancy/lib/adapter/base.py
--rw-r--r--   0        0        0     2680 2023-08-03 08:27:58.698062 feedancy-0.1.7/feedancy/lib/adapter/httpx.py
--rw-r--r--   0        0        0     2446 2023-08-03 08:27:58.699357 feedancy-0.1.7/feedancy/lib/adapter/params_converter.py
--rw-r--r--   0        0        0     3005 2023-08-03 08:27:58.700130 feedancy-0.1.7/feedancy/lib/adapter/requests.py
--rw-r--r--   0        0        0     2769 2023-08-03 08:27:58.695317 feedancy-0.1.7/feedancy/lib/base.py
--rw-r--r--   0        0        0      685 2023-08-03 08:27:58.689083 feedancy-0.1.7/feedancy/lib/client.py
--rw-r--r--   0        0        0      929 2023-08-03 08:27:58.688122 feedancy-0.1.7/feedancy/lib/configuration.py
--rw-r--r--   0        0        0      466 2023-08-03 08:27:58.693065 feedancy-0.1.7/feedancy/lib/exceptions.py
--rw-r--r--   0        0        0      403 2023-08-03 08:27:58.694622 feedancy-0.1.7/feedancy/lib/json.py
--rw-r--r--   0        0        0      613 2023-08-03 08:27:58.689875 feedancy-0.1.7/feedancy/lib/request.py
--rw-r--r--   0        0        0      384 2023-08-03 08:27:58.691206 feedancy-0.1.7/feedancy/lib/response.py
--rw-r--r--   0        0        0      895 2023-08-03 08:27:58.693857 feedancy-0.1.7/feedancy/lib/response_deserializer.py
--rw-r--r--   0        0        0      564 2023-08-03 08:27:58.691988 feedancy-0.1.7/feedancy/lib/types.py
--rw-r--r--   0        0        0      651 2023-08-03 08:27:55.735658 feedancy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-08-08 20:16:26.856117 feedancy-0.1.8/README.md
+-rw-r--r--   0        0        0      126 2023-08-08 20:16:26.823324 feedancy-0.1.8/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:16:26.609114 feedancy-0.1.8/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:16:26.609243 feedancy-0.1.8/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    11875 2023-08-08 20:16:26.615497 feedancy-0.1.8/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      896 2023-08-08 20:16:26.639793 feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-08-08 20:16:26.641847 feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      853 2023-08-08 20:16:26.638968 feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      908 2023-08-08 20:16:26.640525 feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-08 20:16:26.641281 feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      907 2023-08-08 20:16:26.643636 feedancy-0.1.8/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-08-08 20:16:26.646844 feedancy-0.1.8/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      874 2023-08-08 20:16:26.642644 feedancy-0.1.8/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      929 2023-08-08 20:16:26.644512 feedancy-0.1.8/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      961 2023-08-08 20:16:26.645836 feedancy-0.1.8/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0     1258 2023-08-08 20:16:26.649941 feedancy-0.1.8/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-08-08 20:16:26.654077 feedancy-0.1.8/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0     1222 2023-08-08 20:16:26.648172 feedancy-0.1.8/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0     1277 2023-08-08 20:16:26.651073 feedancy-0.1.8/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0     1312 2023-08-08 20:16:26.653377 feedancy-0.1.8/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      899 2023-08-08 20:16:26.655555 feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-08-08 20:16:26.658106 feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-08-08 20:16:26.654796 feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-08-08 20:16:26.656509 feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-08-08 20:16:26.657350 feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      935 2023-08-08 20:16:26.661243 feedancy-0.1.8/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-08-08 20:16:26.666110 feedancy-0.1.8/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      899 2023-08-08 20:16:26.659530 feedancy-0.1.8/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      954 2023-08-08 20:16:26.663412 feedancy-0.1.8/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-08 20:16:26.665196 feedancy-0.1.8/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      876 2023-08-08 20:16:26.667881 feedancy-0.1.8/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-08-08 20:16:26.670584 feedancy-0.1.8/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      840 2023-08-08 20:16:26.666972 feedancy-0.1.8/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      895 2023-08-08 20:16:26.668813 feedancy-0.1.8/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      930 2023-08-08 20:16:26.669707 feedancy-0.1.8/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      881 2023-08-08 20:16:26.672950 feedancy-0.1.8/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-08-08 20:16:26.676825 feedancy-0.1.8/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      844 2023-08-08 20:16:26.671662 feedancy-0.1.8/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      899 2023-08-08 20:16:26.674155 feedancy-0.1.8/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      935 2023-08-08 20:16:26.675651 feedancy-0.1.8/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0     1981 2023-08-08 20:16:26.683539 feedancy-0.1.8/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     2000 2023-08-08 20:16:26.692637 feedancy-0.1.8/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0     1942 2023-08-08 20:16:26.678917 feedancy-0.1.8/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1997 2023-08-08 20:16:26.685866 feedancy-0.1.8/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     2035 2023-08-08 20:16:26.690410 feedancy-0.1.8/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      935 2023-08-08 20:16:26.695204 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-08-08 20:16:26.698937 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      889 2023-08-08 20:16:26.693799 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      944 2023-08-08 20:16:26.696612 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-08 20:16:26.697995 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      923 2023-08-08 20:16:26.701305 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-08-08 20:16:26.705859 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      879 2023-08-08 20:16:26.700042 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      934 2023-08-08 20:16:26.702890 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      977 2023-08-08 20:16:26.704767 feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0     1627 2023-08-08 20:16:26.711206 feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-08-08 20:16:26.717759 feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0     1590 2023-08-08 20:16:26.707658 feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0     1645 2023-08-08 20:16:26.713160 feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0     1681 2023-08-08 20:16:26.716614 feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      874 2023-08-08 20:16:26.719991 feedancy-0.1.8/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-08-08 20:16:26.723495 feedancy-0.1.8/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      839 2023-08-08 20:16:26.718812 feedancy-0.1.8/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      894 2023-08-08 20:16:26.721123 feedancy-0.1.8/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      928 2023-08-08 20:16:26.722427 feedancy-0.1.8/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      969 2023-08-08 20:16:26.726483 feedancy-0.1.8/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-08-08 20:16:26.730734 feedancy-0.1.8/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      953 2023-08-08 20:16:26.724940 feedancy-0.1.8/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0     1008 2023-08-08 20:16:26.728145 feedancy-0.1.8/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0     1023 2023-08-08 20:16:26.729811 feedancy-0.1.8/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      966 2023-08-08 20:16:26.733019 feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-08-08 20:16:26.737257 feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      916 2023-08-08 20:16:26.731780 feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      971 2023-08-08 20:16:26.734247 feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0     1020 2023-08-08 20:16:26.735780 feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      896 2023-08-08 20:16:26.739838 feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-08-08 20:16:26.744401 feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      890 2023-08-08 20:16:26.738590 feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      945 2023-08-08 20:16:26.741176 feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-08 20:16:26.743492 feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      851 2023-08-08 20:16:26.751281 feedancy-0.1.8/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-08-08 20:16:26.758862 feedancy-0.1.8/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      817 2023-08-08 20:16:26.745372 feedancy-0.1.8/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      872 2023-08-08 20:16:26.753788 feedancy-0.1.8/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      905 2023-08-08 20:16:26.757572 feedancy-0.1.8/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      856 2023-08-08 20:16:26.761381 feedancy-0.1.8/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-08-08 20:16:26.766195 feedancy-0.1.8/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      821 2023-08-08 20:16:26.760146 feedancy-0.1.8/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      876 2023-08-08 20:16:26.762838 feedancy-0.1.8/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      910 2023-08-08 20:16:26.764946 feedancy-0.1.8/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      886 2023-08-08 20:16:26.768787 feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-08-08 20:16:26.771726 feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      845 2023-08-08 20:16:26.767446 feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      900 2023-08-08 20:16:26.769933 feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      940 2023-08-08 20:16:26.771086 feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2393 2023-08-08 20:16:26.781816 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2492 2023-08-08 20:16:26.805239 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3540 2023-08-08 20:16:26.775470 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2489 2023-08-08 20:16:26.790042 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2447 2023-08-08 20:16:26.802249 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0     1039 2023-08-08 20:16:26.808074 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-08-08 20:16:26.812574 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      996 2023-08-08 20:16:26.806567 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0     1051 2023-08-08 20:16:26.809368 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0     1093 2023-08-08 20:16:26.811416 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      905 2023-08-08 20:16:26.815448 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-08-08 20:16:26.820731 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      864 2023-08-08 20:16:26.813977 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      919 2023-08-08 20:16:26.817424 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      959 2023-08-08 20:16:26.819810 feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-08-08 20:16:26.831746 feedancy-0.1.8/feedancy/client.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:16:26.836443 feedancy-0.1.8/feedancy/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:16:26.844395 feedancy-0.1.8/feedancy/lib/adapter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-08-08 20:16:26.843184 feedancy-0.1.8/feedancy/lib/adapter/aiohttp.py
+-rw-r--r--   0        0        0      235 2023-08-08 20:16:26.847337 feedancy-0.1.8/feedancy/lib/adapter/base.py
+-rw-r--r--   0        0        0     2680 2023-08-08 20:16:26.843927 feedancy-0.1.8/feedancy/lib/adapter/httpx.py
+-rw-r--r--   0        0        0     2446 2023-08-08 20:16:26.845429 feedancy-0.1.8/feedancy/lib/adapter/params_converter.py
+-rw-r--r--   0        0        0     3005 2023-08-08 20:16:26.846371 feedancy-0.1.8/feedancy/lib/adapter/requests.py
+-rw-r--r--   0        0        0     2769 2023-08-08 20:16:26.841503 feedancy-0.1.8/feedancy/lib/base.py
+-rw-r--r--   0        0        0      685 2023-08-08 20:16:26.835374 feedancy-0.1.8/feedancy/lib/client.py
+-rw-r--r--   0        0        0      929 2023-08-08 20:16:26.834399 feedancy-0.1.8/feedancy/lib/configuration.py
+-rw-r--r--   0        0        0      466 2023-08-08 20:16:26.838911 feedancy-0.1.8/feedancy/lib/exceptions.py
+-rw-r--r--   0        0        0      403 2023-08-08 20:16:26.840604 feedancy-0.1.8/feedancy/lib/json.py
+-rw-r--r--   0        0        0      613 2023-08-08 20:16:26.836100 feedancy-0.1.8/feedancy/lib/request.py
+-rw-r--r--   0        0        0      384 2023-08-08 20:16:26.837283 feedancy-0.1.8/feedancy/lib/response.py
+-rw-r--r--   0        0        0      895 2023-08-08 20:16:26.839919 feedancy-0.1.8/feedancy/lib/response_deserializer.py
+-rw-r--r--   0        0        0      564 2023-08-08 20:16:26.838143 feedancy-0.1.8/feedancy/lib/types.py
+-rw-r--r--   0        0        0      651 2023-08-08 20:15:40.864067 feedancy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.8/PKG-INFO
```

### Comparing `feedancy-0.1.7/README.md` & `feedancy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api.py` & `feedancy-0.1.8/feedancy/apis/api/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,19 +38,14 @@
 from . import api_v1_currency_update
 from . import api_v1_currency_destroy
 from . import api_v1_internship_retrieve
 from . import api_v1_internship_create
 from . import api_v1_internship_retrieve_2
 from . import api_v1_internship_update
 from . import api_v1_internship_destroy
-from . import api_v1_internshipcity_retrieve
-from . import api_v1_internshipcity_create
-from . import api_v1_internshipcity_retrieve_2
-from . import api_v1_internshipcity_update
-from . import api_v1_internshipcity_destroy
 from . import api_v1_internshipcontact_retrieve
 from . import api_v1_internshipcontact_create
 from . import api_v1_internshipcontact_retrieve_2
 from . import api_v1_internshipcontact_update
 from . import api_v1_internshipcontact_destroy
 from . import api_v1_internshipskill_retrieve
 from . import api_v1_internshipskill_create
@@ -98,19 +93,14 @@
 from . import api_v1_stopkeywords_update
 from . import api_v1_stopkeywords_destroy
 from . import api_v1_vacancy_list
 from . import api_v1_vacancy_create
 from . import api_v1_vacancy_retrieve
 from . import api_v1_vacancy_update
 from . import api_v1_vacancy_destroy
-from . import api_v1_vacancycity_retrieve
-from . import api_v1_vacancycity_create
-from . import api_v1_vacancycity_retrieve_2
-from . import api_v1_vacancycity_update
-from . import api_v1_vacancycity_destroy
 from . import api_v1_vacancycontact_retrieve
 from . import api_v1_vacancycontact_create
 from . import api_v1_vacancycontact_retrieve_2
 from . import api_v1_vacancycontact_update
 from . import api_v1_vacancycontact_destroy
 from . import api_v1_vacancyskill_retrieve
 from . import api_v1_vacancyskill_create
@@ -154,19 +144,14 @@
     api_v1_currency_update = api_v1_currency_update.make_request
     api_v1_currency_destroy = api_v1_currency_destroy.make_request
     api_v1_internship_retrieve = api_v1_internship_retrieve.make_request
     api_v1_internship_create = api_v1_internship_create.make_request
     api_v1_internship_retrieve_2 = api_v1_internship_retrieve_2.make_request
     api_v1_internship_update = api_v1_internship_update.make_request
     api_v1_internship_destroy = api_v1_internship_destroy.make_request
-    api_v1_internshipcity_retrieve = api_v1_internshipcity_retrieve.make_request
-    api_v1_internshipcity_create = api_v1_internshipcity_create.make_request
-    api_v1_internshipcity_retrieve_2 = api_v1_internshipcity_retrieve_2.make_request
-    api_v1_internshipcity_update = api_v1_internshipcity_update.make_request
-    api_v1_internshipcity_destroy = api_v1_internshipcity_destroy.make_request
     api_v1_internshipcontact_retrieve = api_v1_internshipcontact_retrieve.make_request
     api_v1_internshipcontact_create = api_v1_internshipcontact_create.make_request
     api_v1_internshipcontact_retrieve_2 = api_v1_internshipcontact_retrieve_2.make_request
     api_v1_internshipcontact_update = api_v1_internshipcontact_update.make_request
     api_v1_internshipcontact_destroy = api_v1_internshipcontact_destroy.make_request
     api_v1_internshipskill_retrieve = api_v1_internshipskill_retrieve.make_request
     api_v1_internshipskill_create = api_v1_internshipskill_create.make_request
@@ -214,19 +199,14 @@
     api_v1_stopkeywords_update = api_v1_stopkeywords_update.make_request
     api_v1_stopkeywords_destroy = api_v1_stopkeywords_destroy.make_request
     api_v1_vacancy_list = api_v1_vacancy_list.make_request
     api_v1_vacancy_create = api_v1_vacancy_create.make_request
     api_v1_vacancy_retrieve = api_v1_vacancy_retrieve.make_request
     api_v1_vacancy_update = api_v1_vacancy_update.make_request
     api_v1_vacancy_destroy = api_v1_vacancy_destroy.make_request
-    api_v1_vacancycity_retrieve = api_v1_vacancycity_retrieve.make_request
-    api_v1_vacancycity_create = api_v1_vacancycity_create.make_request
-    api_v1_vacancycity_retrieve_2 = api_v1_vacancycity_retrieve_2.make_request
-    api_v1_vacancycity_update = api_v1_vacancycity_update.make_request
-    api_v1_vacancycity_destroy = api_v1_vacancycity_destroy.make_request
     api_v1_vacancycontact_retrieve = api_v1_vacancycontact_retrieve.make_request
     api_v1_vacancycontact_create = api_v1_vacancycontact_create.make_request
     api_v1_vacancycontact_retrieve_2 = api_v1_vacancycontact_retrieve_2.make_request
     api_v1_vacancycontact_update = api_v1_vacancycontact_update.make_request
     api_v1_vacancycontact_destroy = api_v1_vacancycontact_destroy.make_request
     api_v1_vacancyskill_retrieve = api_v1_vacancyskill_retrieve.make_request
     api_v1_vacancyskill_create = api_v1_vacancyskill_create.make_request
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_country_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
+class Country(BaseModel):
+    code: str 
     name: str 
-    region: int 
 
 def make_request(self: BaseApi,
 
-    __request__: City,
+    __request__: Country,
 
 
-) -> City:
+) -> Country:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
         method="POST",
-        path="/api/v1/city/".format(
+        path="/api/v1/country/".format(
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -39,12 +39,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "application/json": Country,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class City(BaseModel):
     id: int 
     name: str 
-    region: int 
+    region: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
 
+    id: str,
+
 ) -> City:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/city/".format(
+        path="/api/v1/city/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
+class Skill(BaseModel):
     id: int 
     name: str 
-    region: int 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> City:
+) -> Skill:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/city/{id}/".format(
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +41,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "application/json": Skill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_currency_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
+class Currency(BaseModel):
+    code: str 
     name: str 
-    region: int 
 
 def make_request(self: BaseApi,
 
-    __request__: City,
+    __request__: Currency,
 
 
     id: str,
 
-) -> City:
+) -> Currency:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/city/{id}/".format(
+        path="/api/v1/currency/{id}/".format(
             
                 id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
@@ -43,12 +43,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "application/json": Currency,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_company_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_company_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,37 @@
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Country(BaseModel):
     code: str 
+    id: int 
     name: str 
 
 def make_request(self: BaseApi,
 
-    __request__: Country,
 
+    id: str,
 
 ) -> Country:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/country/".format(
+        method="GET",
+        path="/api/v1/country/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Country(BaseModel):
-    code: str 
+class Source(BaseModel):
     id: int 
     name: str 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Country:
+) -> Source:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/country/{id}/".format(
+        path="/api/v1/source/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +41,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "application/json": Source,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_source_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Currency(BaseModel):
-    code: str 
+class Source(BaseModel):
     name: str 
 
 def make_request(self: BaseApi,
 
-    __request__: Currency,
+    __request__: Source,
 
 
-    id: str,
-
-) -> Currency:
+) -> Source:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/currency/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/source/".format(
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -43,12 +38,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "application/json": Source,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internship_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Internship(BaseModel):
+    city: typing.Optional[typing.Union[int, None]]  = None
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     is_paid: typing.Optional[typing.Union[bool, None]]  = None
@@ -30,24 +31,28 @@
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
     __request__: Internship,
 
 
+    id: str,
+
 ) -> Internship:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/internship/".format(
+        method="PUT",
+        path="/api/v1/internship/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Internship(BaseModel):
+    city: typing.Optional[typing.Union[int, None]]  = None
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Internship(BaseModel):
+    city: typing.Optional[typing.Union[int, None]]  = None
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Internship(BaseModel):
+    city: typing.Optional[typing.Union[int, None]]  = None
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internship_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class Internship(BaseModel):
+    city: typing.Optional[typing.Union[int, None]]  = None
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     is_paid: typing.Optional[typing.Union[bool, None]]  = None
@@ -30,28 +31,24 @@
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
     __request__: Internship,
 
 
-    id: str,
-
 ) -> Internship:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/internship/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/internship/".format(
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,46 +5,45 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
+class InternshipContact(BaseModel):
+    contact: int 
+    id: int 
     internship: int 
 
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
 
-
-) -> InternshipCity:
+) -> InternshipContact:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/internshipcity/".format(
+        method="GET",
+        path="/api/v1/internshipcontact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "application/json": InternshipContact,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/api/v1/internshipcity/{id}/".format(
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
+class Region(BaseModel):
+    country: int 
     id: int 
-    internship: int 
+    name: str 
 
 def make_request(self: BaseApi,
 
 
-) -> InternshipCity:
+) -> Region:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipcity/".format(
+        path="/api/v1/region/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +38,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "application/json": Region,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,36 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
+class InternshipSkill(BaseModel):
     id: int 
     internship: int 
+    skill: int 
 
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> InternshipCity:
+) -> InternshipSkill:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipcity/{id}/".format(
-            
-                id=id,
+        path="/api/v1/internshipskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +38,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "application/json": InternshipSkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,49 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
+class InternshipSkill(BaseModel):
+    id: int 
     internship: int 
+    skill: int 
 
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
-
 
     id: str,
 
-) -> InternshipCity:
+) -> InternshipSkill:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/internshipcity/{id}/".format(
+        method="GET",
+        path="/api/v1/internshipskill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "application/json": InternshipSkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_source_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,45 +5,49 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    id: int 
-    internship: int 
+class Source(BaseModel):
+    name: str 
 
 def make_request(self: BaseApi,
 
+    __request__: Source,
 
-) -> InternshipContact:
+
+    id: str,
+
+) -> Source:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/internshipcontact/".format(
+        method="PUT",
+        path="/api/v1/source/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "application/json": Source,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_region_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
+class Region(BaseModel):
+    country: int 
     id: int 
-    internship: int 
-    skill: int 
+    name: str 
 
 def make_request(self: BaseApi,
 
 
-) -> InternshipSkill:
+    id: str,
+
+) -> Region:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipskill/".format(
+        path="/api/v1/region/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +42,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "application/json": Region,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class InternshipSkill(BaseModel):
-    id: int 
     internship: int 
     skill: int 
 
 def make_request(self: BaseApi,
 
+    __request__: InternshipSkill,
+
 
     id: str,
 
 ) -> InternshipSkill:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
+        method="PUT",
         path="/api/v1/internshipskill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_source_retrieve.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
-    internship: int 
-    skill: int 
+class Source(BaseModel):
+    id: int 
+    name: str 
 
 def make_request(self: BaseApi,
 
-    __request__: InternshipSkill,
 
-
-    id: str,
-
-) -> InternshipSkill:
+) -> Source:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/internshipskill/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/source/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "application/json": Source,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_jobmixin_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_skill_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
-    id: int 
+class Skill(BaseModel):
     name: str 
 
 def make_request(self: BaseApi,
 
+    __request__: Skill,
 
-) -> Region:
+
+) -> Skill:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/region/".format(
+        method="POST",
+        path="/api/v1/skill/".format(
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "application/json": Skill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
+class StopKeywords(BaseModel):
     id: int 
     name: str 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Region:
+) -> StopKeywords:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/region/{id}/".format(
+        path="/api/v1/stopkeywords/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +41,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "application/json": StopKeywords,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_salary_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_salary_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_salary_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
-    name: str 
+class VacancySkill(BaseModel):
+    skill: int 
+    vacancy: int 
 
 def make_request(self: BaseApi,
 
-    __request__: Skill,
+    __request__: VacancySkill,
 
 
-) -> Skill:
+    id: str,
+
+) -> VacancySkill:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/skill/".format(
+        method="PUT",
+        path="/api/v1/vacancyskill/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +43,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "application/json": VacancySkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/api/v1/skill/{id}/".format(
+        path="/api/v1/source/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
+class VacancySkill(BaseModel):
     id: int 
-    name: str 
+    skill: int 
+    vacancy: int 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Skill:
+) -> VacancySkill:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/skill/{id}/".format(
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +42,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "application/json": VacancySkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_city_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
+class City(BaseModel):
     name: str 
+    region: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Source,
+    __request__: City,
 
 
-) -> Source:
+    id: str,
+
+) -> City:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/source/".format(
+        method="PUT",
+        path="/api/v1/city/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +43,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "application/json": City,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/api/v1/source/{id}/".format(
+        path="/api/v1/vacancycontact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
+class City(BaseModel):
     id: int 
     name: str 
+    region: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
 
-) -> Source:
+) -> City:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/source/".format(
+        path="/api/v1/city/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +38,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "application/json": City,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,35 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
+class StopKeywords(BaseModel):
     id: int 
     name: str 
 
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Source:
+) -> StopKeywords:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/source/{id}/".format(
-            
-                id=id,
+        path="/api/v1/stopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -41,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "application/json": StopKeywords,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,33 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
-    name: str 
+class VacancySkill(BaseModel):
+    skill: int 
+    vacancy: int 
 
 def make_request(self: BaseApi,
 
-    __request__: Source,
+    __request__: VacancySkill,
 
 
-    id: str,
-
-) -> Source:
+) -> VacancySkill:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/source/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancyskill/".format(
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +39,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "application/json": VacancySkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,38 @@
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 class StopKeywords(BaseModel):
-    id: int 
     name: str 
 
 def make_request(self: BaseApi,
 
+    __request__: StopKeywords,
+
+
+    id: str,
 
 ) -> StopKeywords:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/stopkeywords/".format(
+        method="PUT",
+        path="/api/v1/stopkeywords/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,33 +5,38 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
+class Contact(BaseModel):
+    data: str 
     id: int 
-    name: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> StopKeywords:
+) -> VacancyContact:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/stopkeywords/{id}/".format(
+        path="/api/v1/vacancycontact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +46,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "application/json": VacancyContact,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,34 +5,39 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
-    name: str 
+class Contact(BaseModel):
+    data: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
 
 def make_request(self: BaseApi,
 
-    __request__: StopKeywords,
+    __request__: VacancyContact,
 
 
     id: str,
 
-) -> StopKeywords:
+) -> VacancyContact:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/stopkeywords/{id}/".format(
+        path="/api/v1/vacancycontact/{id}/".format(
             
                 id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
@@ -42,12 +47,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "application/json": VacancyContact,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
+    city: str 
     company: typing.Union[str, None] 
     contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_list.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
+    city: str 
     company: typing.Union[str, None] 
     contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_retrieve.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
+    city: str 
     company: typing.Union[str, None] 
     contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancy_update.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,46 +5,45 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyCity(BaseModel):
-    city: int 
+class VacancySkill(BaseModel):
+    id: int 
+    skill: int 
     vacancy: int 
 
 def make_request(self: BaseApi,
 
-    __request__: VacancyCity,
 
-
-) -> VacancyCity:
+) -> VacancySkill:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/vacancycity/".format(
+        method="GET",
+        path="/api/v1/vacancyskill/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "application/json": VacancySkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/api/v1/vacancycity/{id}/".format(
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_city_create.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,49 +5,46 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    id: int 
-    vacancy: int 
+class City(BaseModel):
+    name: str 
+    region: typing.Optional[typing.Union[int, None]]  = None
 
 def make_request(self: BaseApi,
 
+    __request__: City,
 
-    id: str,
 
-) -> VacancyCity:
+) -> City:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/vacancycity/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/city/".format(
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "application/json": City,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.1.8/feedancy/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,44 +5,49 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-def make_request(self: BaseApi,
+class Contact(BaseModel):
+    data: str 
+    id: int 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
 
+def make_request(self: BaseApi,
 
-    id: str,
 
-) -> None:
+) -> VacancyContact:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/api/v1/vacancycontact/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/vacancycontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
-                "default": None,
+                "application/json": VacancyContact,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.7/feedancy/client.py` & `feedancy-0.1.8/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/adapter/aiohttp.py` & `feedancy-0.1.8/feedancy/lib/adapter/aiohttp.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/adapter/httpx.py` & `feedancy-0.1.8/feedancy/lib/adapter/httpx.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/adapter/params_converter.py` & `feedancy-0.1.8/feedancy/lib/adapter/params_converter.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/adapter/requests.py` & `feedancy-0.1.8/feedancy/lib/adapter/requests.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/base.py` & `feedancy-0.1.8/feedancy/lib/base.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/client.py` & `feedancy-0.1.8/feedancy/lib/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/configuration.py` & `feedancy-0.1.8/feedancy/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/request.py` & `feedancy-0.1.8/feedancy/lib/request.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/response_deserializer.py` & `feedancy-0.1.8/feedancy/lib/response_deserializer.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/feedancy/lib/types.py` & `feedancy-0.1.8/feedancy/lib/types.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.7/pyproject.toml` & `feedancy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feedancy"
-version = "0.1.7"
+version = "0.1.8"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `feedancy-0.1.7/PKG-INFO` & `feedancy-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.1.7
+Version: 0.1.8
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

