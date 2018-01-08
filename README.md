# Evergreen
Evergreen dev project

Scope
* Develop a course/pathway marketplace
* Feed with Evergreen content (network generated and seed) and API sources
* allow students to enroll and complete courses
* facilitate provider course manager/admin 


Use cases
* Student search: keyword, topic, pathway, related, local
* Student Pathway search: current, topic/industry, education level

Project breakdown
* Views (workflows)
  * Marketplace home
  * Course Explorer
  * Pathway Explorer
Controller
  * PromoPathway query (mkt_home)
  * pathway_topic query (pathway_explorer)
  * current_pathway query (pathway_explorer; current + any added)
  * grade_search (pathway_explorer; overlay pathways)
  * pathway_add (pathway_explorer)
  * course_search query (course_explorer)
  * course_list
  * course_map
  * course_detail
  * course_grade_enroll
  * Grade.create
  * Grade.enroll
  * grade.complete
  * course_pathway_preview
* Models
  * Course.search{ Course.evgSearch, Course.apiSearch}
  * Course.grade
  * Course.
  * Pathway


Sample datasets
* Courses
  * MSN HS
  * MSN Technical
  * MSN 4yr
  * MSN Community
  * Khan acadmey API search
* Pathways
  * 1 trade - plumbing
  * 1 industry - healthcare (nursing/physician)
  * 1 HS > 4yr
  * 1 HS > 2yr > 4yr



After the MVP
* add backpack through grades
* Develop Gradebook integration
  * course_reg, course_enroll, course_grade
* Develop parent-proxy support
* Increase scope of API search
* Develop export features
* Increase pathway queries
* Increase pathway datasets
* add blockchain through grades
* add cellular support


API searches
* Only for 'course' search to begin with
** Must list on Evergreen to be included in pathways? Or eventual inclusion?
* Use https://api-explorer.khanacademy.org/group/api/v1/topic ?
