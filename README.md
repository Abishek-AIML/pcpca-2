Please find your credentials and instructions for the CA2 React Assessment below:

Credentials
Password: 279539

Test Server Details
- Base URL: https://t4e-testserver.onrender.com/api

Mandatory Instructions

1. Authentication & Data Fetch: Ensure proper integration using the API → Context → Reducer architecture.
2. Routing: Implement the following routes exactly as specified, including their corresponding ID, /filter, and /stats routes. Route names must match exactly to pass evaluation.
3. Test IDs: Use the mandatory data-testid attributes for list rendering, filter inputs, and the stats page as outlined in your assessment requirements.
List Rendering:

data-testid="order-item" / activity-item / course-item / event-item
Filter:

data-testid="filter-input"
Stats Page:

data-testid="total-orders" / total-activities / total-courses / total-events
data-testid="delivered-orders" / goal-achieved / active-courses / active-events
data-testid="cancelled-orders" / goal-not-achieved / inactive-courses / soldout-events
4. Global State: In the Stats component, you must expose the window.appState object containing all required count metrics.
5. Deployment (Vercel): Create a vercel.json file in the root folder with the necessary rewrite rules to handle client-side routing.

{
  "rewrites": [
    {
      "source": "/((?!assets|.*\\..*).*)",
      "destination": "/index.html"
    }
  ]
}


Submission
Deploy your project to Vercel and submit the live URL via this form: https://forms.gle/R2HyM8hexjAKcuot6.
Submissions must be completed on or before 8:45 a.m.

Important Notes
- Strictly follow Context and Reducer architecture.
- Use reduce or filter rather than storing derived values.
- Handle inconsistent data and maintain clean code.

If you encounter any issues during the assessment, please contact the trainer immediately.
