# FA7 Group Project Submission

## Group Members
* Diche, Jasmine
* Hermosada, Joshua

---

## Part 1: Exponential Distribution (Student Arrival Gaps at Campus Gate)

### Project Summary
We tracked the time gaps between individual students arriving at Gate 4 of our university campus. Our goal was to see if these arrival time gaps follow an Exponential Distribution model, which helps us understand how smoothly students flow into campus.

### How We Collected the Data (Methodology)
* We chose **Seconds Between Student Arrivals** as our quantitative variable.
* We sat near Gate 4 on an afternoon starting at **2:30 PM** (30 minutes before the busy 3:00 PM class transition period).
* We used a smartphone stopwatch application and clicked the **"Lap"** feature every time a student walked through the gate to capture a natural flow of consecutive arrivals.
* We recorded **30 data points** in total.

### Our Results and Math Stats
After running our stopwatch numbers through R, here is what our data showed:

* **Total Arrivals Recorded:** 30 students
* **Average Gap Between Students (Mean):** 13.17 seconds
* **Lambda (Arrival Rate):** 0.07595 students arriving per second

#### Assumptions Verified
1. **Randomness:** Students walk into campus individually based on their own personal schedules and habits, making the exact timing random.
2. **Independence:** One student walking through the gate does not cause or stop another student from entering. Each person arrives completely independently of the next.

#### Probability Calculation
Using our cumulative distribution formula, we calculated the likelihood of student spacing:
* There is a **53.21% chance** that a new student will arrive within **10 seconds** or less of the previous student.

### Data Interpretation and Real-World Usefulness
* **What it Implies:** The data follows a smooth exponential curve where very short gaps (between 0 and 10 seconds) are highly frequent. Long gaps over 30 seconds are rare.
* **How is this useful in real life?** 
  * **For Campus Security & Staff:** Because the traffic flow is a steady, continuous stream of rapid individual arrivals rather than massive sudden clusters, gate security and check-in staff need to be consistently alert to process individual entry passes quickly one by one. This keeps gate entry manageable and prevents traffic from backing up.

---

## Part 2: Normal Distribution (Student Lunch Money Project)

### Project Summary
We wanted to see how much money students get for lunch every day and check if it follows a Normal Distribution curve. Our goal was to find the average lunch budget on campus and see how student allowances are spread out.

### How We Collected the Data (Methodology)
* We chose **Lunch Money Allotment** as our quantitative variable.
* We asked **50 students** verbally on campus how much money they get for lunch.
* To respect privacy, we kept it totally anonymous. We didn't list any names, just numbered the students 1 to 50 in our Excel file (`fa7.xlsx`).
* We imported our data into R using VS Code to do all our math calculations and make our charts.

### Our Results and Math Stats
After running our code in R, here is what we found from our 50 students:

* **Total Students Surveyed:** 50
* **Average (Mean) Lunch Money:** 165.00 PHP
* **Sample Standard Deviation:** 66.43 PHP
* **Population Standard Deviation:** 65.76 PHP

#### Frequency Table (How many students are in each price range)
* 80 PHP: 4 students (8%)
* 100 PHP: 8 students (16%)
* 120 PHP: 10 students (20%)
* 150 PHP: 9 students (18%)
* 200 PHP: 7 students (14%)
* 250 PHP: 6 students (12%)
* 280 PHP: 6 students (12%)
Total: 50 students (100%)

#### Checking the Empirical Rule (68-95-99.7 Rule)
* **Within 1 Standard Deviation (99.24 to 230.76 PHP):** Exactly 68.00% of our students fall in this range. This matches a perfect normal distribution model exactly!
* **Within 2 Standard Deviations (33.47 to 296.53 PHP):** 100.00% of our students fall here.
* **Within 3 Standard Deviations (-32.29 to 362.29 PHP):** 100.00% of our students fall here.

### Interpretation

* **Is the distribution symmetric?** Yes, it is pretty well-balanced! There are 22 students who have below average budgets and 19 students who have above average budgets, with 9 students right in the middle. It has a bit of a flat top, but both sides match up nicely on the graph.
* **Are there outliers?** No, we have zero outliers. Since 100% of our students fit inside 2 standard deviations, nobody had an insanely huge or tiny lunch budget that ruined the chart.
* **What does the shape of the distribution imply?** The flat-topped shape means student allowances are spread out evenly across different budgets. We don't have everyone clustering around just one amount; campus has a big mix of low, middle, and high-allowance students.
* **How can this data be useful?** 
  * **For Food Vendors:** Since 68% of students have a budget between roughly 99 PHP and 231 PHP, canteen stalls will make the most sales if they price their combo meals around 120 PHP to 150 PHP.
  * **For the School Welfare Committee:** We noticed that 24% of our surveyed students have a lunch budget of 100 PHP or less. This shows that the school needs to keep affordable, cheap meal options available so these students can still buy food.
