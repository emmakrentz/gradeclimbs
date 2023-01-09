# Using ML to automatically grade indoor top rope rock climbing routes.
An enduring problem in both indoor and outdoor rock climbing is the non-standardization of climbing grades in all disciplines, including bouldering, top-roping, and lead climbing.
<p>
Indoor top rope climbs in North America are typically graded using the Yosemite Decimal System (YDS), which grades climbs from 5.1 to 5.15, with sublevels of the form 5.x(a/b/c/d) for climbs starting at the level 5.10. Thus a 5.10b is more difficult than a 5.10a (neither of which as difficult as a 5.11a).  (https://www.rei.com/learn/expert-advice/climbing-bouldering-rating.html)
<p>
Outdoor climbs are typically assigned a grade upon their first ascent (FA), by the climber who first climbed them. This rating may change as more ascents are completed and climbers of various strengths attempt the routes. Especially famous and popular routes have grades that are virtually cemented as more and more ascents are put up. There is often news in the climbing community when a climber downgrades a difficult route upon a second ascent (https://www.climbing.com/news/stefano-ghisolfi-downgrades-bibliographie-5-15c/). 
<p>
In indoor climbing gyms, grading can be even more subjective. Grades are typically assigned by a small team of routesetters who often set (and even climb) at only one gym. Since routes are cycled through quickly, there is no outdoor luxury of permanence and endless climbers finetuning the grade of a route until it is broadly accepted. As a result, gyms tend to end up in their own insular grading bubble, where a climber who can climb only 5.9 at one gym may find herself sending 5.12b at another.
<p>
Is there a way to use machine learning and image recognition to standardize the indoor top rope grading system?
<p>
First, a few considerations to make:
<ol>
  <li>Types of holds: from the ground, a sloper may resemble a jug: however, a climb of jugs will be significantly easier.
  </li>
  <li>Height of wall: a 20-foot wall will be significantly easier for most climbers than a 60-foot wall.
  </li>
  <li>Steepness: an overhang will be treated differently than a slab wall for most climbers.
  </li>
  <li>Subjectivity: in order to create a target variable, one gym will have to be assumed to have the "correct" grading schema.
  </li>
  <li>Population: photos of routes will have to be taken over a long period of time, as most gyms do not have hundreds of routes up at once. 
  </li>
  <li>Format of photos: must include entire wall, must not show dangling rope, no climbers on wall, must be able to distinguish different colours of holds as different routes.
  </li>
</ol>
