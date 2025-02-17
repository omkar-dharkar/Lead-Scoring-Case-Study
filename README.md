# Lead-Scoring-Case-Study
Team Members:
<div style="background: linear-gradient(to right, #ffd700, #ffcc33); color: #1e272e; padding: 20px; border-radius: 10px; font-family: 'Poppins', sans-serif; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); text-align: center;">
  <h2 style="font-size: 24px; color: #fff; text-shadow: 2px 2px 4px rgba(0,0,0,0.3);">✨ Team Members ✨</h2>
  <p style="font-size: 18px; font-weight: bold; margin-top: 10px;">
    📌 Shifa Sayed<br>
    📌 Shubhankar Chakravarty<br>
    📌 Omkar Dharkar<br>
    📌 Sachin Gaikwad
  </p>
</div> 

<div style="background: #1e272e; color: #f5f5f5; padding: 25px; border-radius: 12px; font-family: 'Poppins', sans-serif; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);">
  
  <h1 style="text-align: center; font-size: 32px; color: #ffcc80; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">📊 Logistic Regression Case Study</h1>
  <h2 style="text-align: center; font-size: 24px; color: #81d4fa;">Lead Scoring for X Education</h2>
  
  <hr style="border: none; height: 2px; background: linear-gradient(to right, #ffcc80, #ff8a65); margin: 20px 0;">
  
  <h3 style="color: #64ffda;">🚀 Problem Statement</h3>
  <p style="font-size: 16px; line-height: 1.8;">
     An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses.

The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos.
When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals.
Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%.

Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, **the company wishes to identify the most potential leads, also known as ‘Hot Leads’**.
If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. A typical lead conversion process can be represented using the following funnel:
  </p>
  <img src="https://cdn.upgrad.com/UpGrad/temp/189f213d-fade-4fe4-b506-865f1840a25a/XNote_201901081613670.jpg">
    <br>
    As you can see, there are a lot of leads generated in the initial stage (top) but only a few of them come out as paying customers from the bottom.
In the middle stage, you need to nurture the potential leads well (i.e. educating the leads about the product, constantly communicating etc. ) in order to get a higher lead conversion.

X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers.The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance.<b>The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.</b>
<br><br>
  <div style="background: #263238; padding: 15px; border-radius: 8px; box-shadow: inset 0 0 10px rgba(255, 255, 255, 0.1);">
    <p style="font-size: 16px; line-height: 1.6; color: #ffcc80;">
      🔹 Too many leads, making manual filtering inefficient.<br>
      🔹 Wasted resources on low-converting leads.<br>
      🔹 Need for a <b>data-driven lead scoring system</b>.
    </p>
  </div>

  <h3 style="color: #64ffda; margin-top: 20px;">🎯 Business Objective</h3>
  <p style="font-size: 16px; line-height: 1.8;">
    The goal is to develop an <b>AI-powered Lead Scoring Model</b> that assigns a <b>conversion probability score (0-100)</b> to each lead.
  </p>
  
  <div style="background: linear-gradient(to right, #ff8a65, #ffcc80); padding: 15px; border-radius: 8px; box-shadow: inset 0 0 10px rgba(255, 255, 255, 0.2);">
    <p style="font-size: 16px; line-height: 1.6; color: #333;">
      ✅ <b>Hot Leads (High Score)<b> → Higher chance of conversion.<br>
        ✅ <b>Cold Leads (Low Score)</b> → Lower chance of conversion.<br>
        ✅ <b>Increase conversion rate to 80%</b> as per CEO’s target.
    </p>
  </div>

  <h3 style="color: #64ffda; margin-top: 20px;">📊 Dataset Overview</h3>
  <p style="font-size: 16px; line-height: 1.8;">
    The dataset contains <b>~9,000 historical leads</b> with features such as:
  </p>
  
  <ul style="list-style-type: none; padding-left: 0;">
    <li style="background: #37474f; padding: 10px; margin: 5px 0; border-radius: 6px;">📌 <b>Lead Source</b> (Google, Organic Search, Referral, etc.)</li>
    <li style="background: #37474f; padding: 10px; margin: 5px 0; border-radius: 6px;">📌 <b>Time Spent on Website</b> (User engagement)</li>
    <li style="background: #37474f; padding: 10px; margin: 5px 0; border-radius: 6px;">📌 <b>Last Activity</b> (Email Opened, Phone Call, etc.)</li>
    <li style="background: #37474f; padding: 10px; margin: 5px 0; border-radius: 6px;">📌 <b>Converted</b> (Target variable: 1 = Converted, 0 = Not Converted)</li>
  </ul>

  <h3 style="color: #64ffda; margin-top: 20px;">📌 Goal & Expected Outcome</h3>
  <p style="font-size: 16px; line-height: 1.8;">
    🔹 <b>Develop a Logistic Regression Model</b> to predict lead conversion probability.<br>
    🔹 <b>Assign a lead score (0-100)</b> based on probability.<br>
    🔹 Enable <b>data-driven decision-making</b> to maximize conversion efficiency.
  </p>

  <hr style="border: none; height: 2px; background: linear-gradient(to right, #ffcc80, #ff8a65); margin: 20px 0;">

  <p style="text-align: center; font-size: 18px; font-weight: bold; color: #ffcc80;">
    🎯 This model will **increase conversion rates, optimize sales efforts, and boost revenue!** 📈
  </p>

</div>
