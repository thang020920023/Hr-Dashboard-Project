# Hr-Dashboard-Project

Objectives: Create a report to monitor the human resources situation of the enterprise, tracking the following criteria:

### Page Home:

- Number of employees, number of males, females, and the corresponding ratio
- Number of employees under consideration for a raise or promotion; number of employees not under consideration for a raise or promotion
- Number of employees by years of service
- Number of employees by level
- Number of employees expected to retire, not expected to retire, and the corresponding ratio
- Statistics on the structure of employees based on the distance from home to workplace

### Page Action:

- Detailed list of employees under consideration for promotion
- Detailed list of employees expected to retire

### Page Detail:

- Number of employees under consideration for retirement, and promotion by department
- Number of employees by job satisfaction level
- Percentage of employees working overtime
- Percentage of high-performing and low-performing employees (performance rating)
- Statistics on the total number of employees, number of employees under consideration for promotion, and number of employees under consideration for retirement by job role

### Assumption:

- **Determining employees due for retirement:**
    
    If `[YearsAtCompany] >= 18` then "Due for retirement" else "On service"
    
- **Determining employees due for promotion:**
    
    If `[YearsSinceLastPromotion] >= 10` then "Due for promotion" else "Not due"
    
- **Distance to the workplace:**
    
    If `[DistanceFromHome] >= 20` then "Very Far"
    
    Else if `[DistanceFromHome] >= 10` then "Close"
    
    Else "Very Close"
    
- **Determining job satisfaction level:**
    
    If `[JobSatisfaction] <= 2` then "High"
    
    Else if `[JobSatisfaction] = 3` then "Medium"
    
    Else "Low"
    
- **Determining employee performance rating:**
    
    If `[PerformanceRating] = 3` then "High Ratings"
    
    Else "Low Ratings"
