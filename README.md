# ✈️ Airline Passenger Satisfaction Analysis  

## 📜 Overview  
This project analyzes **passenger satisfaction levels** based on various **service attributes and demographics** using **data visualization techniques** in **R and Tableau**. The study identifies areas needing improvement in airline services to enhance passenger experience.

## 🎯 Problem Explanation  
Airline companies continuously seek ways to **improve customer satisfaction** across different aspects of the flight experience, from **booking tickets** to **baggage claim**. This project focuses on:  
- **Passenger demographics** (age, customer type, class)  
- **Satisfaction levels** across different airline classes  
- **Key service areas for improvement**  

📌 **Dataset**: Kaggle’s Airline Passenger Satisfaction dataset (129,880 observations, 24 attributes).  

## 📊 Data Description  
| **Feature**         | **Description**                        | **Type**         |
|---------------------|------------------------------------|----------------|
| ID                 | Unique passenger identifier       | Numerical      |
| Age                | Passenger's age                   | Numerical      |
| Flight Distance    | Flight distance in miles         | Numerical      |
| Departure Delay    | Delay in minutes                 | Numerical      |
| Arrival Delay      | Delay in minutes                 | Numerical      |
| Gender            | Male / Female                     | Categorical    |
| Customer Type      | First-time / Returning           | Categorical    |
| Type of Travel     | Business / Personal              | Categorical    |
| Class             | Business, Economy Plus, Economy  | Categorical    |
| Satisfaction      | Satisfied / Neutral or Unsatisfied | Categorical    |
| **Survey Ratings** | Ratings (1 to 5) on **14 services** | Ordinal        |

## 🔍 Exploratory Data Analysis  

### **1. Variable Correlation**  
- A **correlation matrix** highlights the relationships between **service quality, delays, and satisfaction**.  
- Strong correlations:  
  - **Seat Comfort & Cleanliness (0.70)** → Enhancing either improves overall satisfaction.  
  - **Online Booking & WiFi Service (0.64)** → Tech-related services impact passenger experience.  
  - **Departure Delay & Arrival Delay (-0.97)** → Addressing departure delays reduces arrival issues.  

📊 **Tools Used**: `ggcorrplot`, `dplyr` (R)  

### **2. Survey Responses Pattern**  
- **Stacked bar graph** shows **50% of survey responses rate services at levels 4 or 5**.  
- **High-rated services**: In-flight Service, Baggage Handling, Seat Comfort.  
- **Low-rated services**: Ease of Online Booking, Gate Location, In-flight Wi-Fi.  
- **Takeaway**: **Technology-related services need improvement.**  

📊 **Tools Used**: Tableau  

### **3. Passenger Distribution**  
- **Majority of returning passengers** are **mid-aged (40-59 years)**.  
- **First-time travelers** are mostly **young adults (18-24 years)**.  
- **Business class has the most returning passengers**.  

📊 **Tools Used**: Tableau  

### **4. Passenger Satisfaction Trends**  
- **Older passengers report higher satisfaction levels.**  
- **Economy and Economy Plus classes** have lower satisfaction scores than Business.  
- **Satisfaction rates: Business > Economy Plus > Economy.**  
- **Booking Services and Pre-Boarding Services receive the lowest ratings across all age groups.**  

📊 **Tools Used**: `ggplot2` (R), Tableau  

## 📈 Explanatory Visualizations  

### **1. Passenger Satisfaction by Age Group & Class**  
📌 **Visuals Used**:  
- **Stacked bar plot** (total passenger count)  
- **Proportional stacked bar plot** (satisfaction percentages)  

📊 **Findings**:  
- **Mid-aged Business class passengers (40-59 years) are most satisfied.**  
- **Economy passengers report the most dissatisfaction.**  

### **2. Service Satisfaction Across Airline Classes**  
📌 **Visuals Used**:  
- **Radar Chart** (Business vs. Economy Plus vs. Economy)  

📊 **Findings**:  
- **Business class scores highest in all service categories.**  
- **Economy has the lowest ratings in essential and flight services.**  

### **3. Service Ratings by Age Group (Economy & Economy Plus)**  
📌 **Visuals Used**:  
- **Box Plot** (Service ratings for different age groups)  

📊 **Findings**:  
- **Booking Services and Pre-Boarding Services receive the lowest ratings.**  
- **Mid-aged passengers give higher ratings across most categories.**  

### **4. Areas Needing Improvement**  
📌 **Visuals Used**:  
- **Heatmap** (Average service ratings by travel type and flight distance)  

📊 **Findings**:  
- **Ease of Online Booking has the lowest ratings, particularly for personal travelers.**  
- **Business passengers give lower ratings to Check-in Service.**  
- **Short-haul flights have lower service ratings than long-haul flights.**  

## 📢 Key Findings & Recommendations  

✅ **Key Findings**:  
- **Older passengers (40+) are more satisfied.**  
- **Business class passengers are the most satisfied, while Economy passengers are least satisfied.**  
- **Booking Services and Pre-Boarding Services are the most criticized.**  

🔧 **Recommendations**:  
- 🎯 **Target loyalty programs for Adults (25-39 years)** to increase retention.  
- 📲 **Improve Online Booking** → Work with third-party vendors for a better experience.  
- ⏳ **Enhance Check-in Service for Business Class** → Streamline boarding efficiency.  
- 🛫 **Upgrade Pre-Boarding Experience** → Improve waiting times, lounge access, and priority boarding.  


## 🚀 Technologies Used  
🛠 **Data Processing & Visualization**:  
- **R** (`ggplot2`, `dplyr`, `tidyverse`) – Exploratory & explanatory analysis  
- **Tableau** – Interactive visualizations  

💾 **Dataset Source**: [[Kaggle - Airline Passenger Satisfaction](https://www.kaggle.com/](https://github.com/pngo1997/Images/blob/main/VS4%20-%20Satisfaction.png))  

## 📊 Sample Visualizations  

### **1. Passenger Satisfaction Distribution**
- Given six Age Groups, the above stacked bar charts display the number of passengers distributed across sub-groups. Noticeably, Adults and Mid Aged passengers (25-59 years old) represent the majority of the data, particularly Mid-Aged passengers flying Business Class with 32,000 passengers, indicating a key demographic for airlines. The proportional stacked bar charts below emphasize the satisfaction level distribution as percentages within each sub-group. The overall pattern shows that satisfaction levels tend to increase with age, showing that older age groups report higher satisfaction with their flight experiences. 
- A notable pattern is that the majority of passengers are more Neutral or Dissatisfied with their flight experience, suggesting that airlines need to review their services and make improvement plans. Indeed, across three classes, Business Class has more Satisfied feedback. This suggests that Business Class services meet the expectations of these passengers better. While Economy and Economy Plus show the same pattern, with slightly higher satisfaction for Economy Plus, which is reasonable considering passengers pay a slight premium for the upgrade.
![Satisfaction Distribution](https://github.com/pngo1997/Images/blob/main/VS%204%20-%20Satisfaction.png)  

### **2. Service Ratings Across Airline Classes**
- The radar chart visualizes service ratings across Business, Economy Plus, and Economy classes, covering aspects like Booking Services, Travel Time Convenience, Post Flight Services, Essential Services, Flight Services, and Pre-Boarding Services. Business class consistently shows higher ratings across all categories, indicating greater passenger satisfaction, especially in Pre Boarding and Post Flight Services. Economy Plus has moderate ratings, higher than Economy but lower than Business, with balanced satisfaction levels. Economy class shows the lowest ratings, particularly in Essential Services and Flight Services, highlighting areas for improvement. Enhancing these specific areas in Economy could significantly elevate overall passenger satisfaction.
![Radar Chart](https://github.com/pngo1997/Images/blob/main/VS%204%20-%20Service%20rating.png)  

### **3. Heatmap of Service Needs Improvement**
- The heatmap reveals several key insights regarding passenger ratings for various services across different travel types and flight distance categories. Notably, Ease of Online Booking is the service with the lowest average ratings across all services, particularly among personal travel passengers. The lowest average rating is observed in the Personal Short-haul category for Ease of Online Booking, with a rating of 2.39. This indicates a significant area for improvement in the online booking process for personal travelers. 
- Interestingly, while business passengers generally provide higher average ratings across most services, the Check-in Service stands out as an exception. Personal travelers, especially in the Short-haul category, rate the Check-in Service higher, with a notable rating of 3.33 compared to business travelers. This suggests that personal travelers find the check-in process more satisfactory, highlighting a potential strength in this service area.
![Service Heatmap](https://github.com/pngo1997/Images/blob/main/VS%204%20-%20Service%20Improvement.png)  

---

## 🏆 Conclusion & Future Scope  
🔍 **Summary**:  
- The **biggest dissatisfaction factors** stem from **online booking, check-in services, and pre-boarding experiences**.  
- The **most satisfied group** consists of **mid-aged, Business Class passengers**.  
- **Future scope** includes adding more datasets with **flight routes, seating configurations, and airline-specific customer feedback.**  
