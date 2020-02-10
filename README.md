Create an object Employee. The class should have the following member variables:
FirstName, LastName, StreetAddress, City, State, Zip, TaxID, Position, Department
Create a database (Room or Sqlite) for the Employee object.
Create the following Activities:
1. MainActivity
  - Make this into a splash screen activity.
  - After any initializations for the applications, start the FilterEmployeeActivity.
2. FilterEmployeeActivity
  - Used a one spinner to select department of the employee. DEPARTMENTS MUST BE RETRIEVED FROM DATABASE.
  - This activity will start the EmployeeListActivity.
3. EmployeeListActivity
  - List all the employees matching the criteria selected in the FilterEmployeeActivity.
  - Implement a Navigation drawer here for the following activities. Since this activities will be also be called from the Employee details activity, you will need to devise a way to get the info for a specific employee both without the employee known and with the employee known.
      - NewEmployeeActivity
      - DeleteEmployeeActivity
      - UpdateEmployeeActivity
      - FilterEmployeeActivity
4. NewEmployeeActivity
  - Allows the user to enter a new employee into the database.
  - Once operation is complete, go back to the Listing activity.
   - When insert is complete, display a toast letting user know which employee was added
5. DeleteEmployeeActivity
  - Allow user to delete an employee from the database.
  - Once operation is complete, go back to the Listing activity.
  - When delete is complete, display a toast letting user know which employee was deleted
6. UpdateEmployeeActivity
  - Allow user toupdate an employee from the database.
  - Once operation is complete, go back to the Listing activity.
  - When update is complete, display a toast letting user know which employee was updated
7. EmployeeDetailsActivity
  - Display all info about the employee.
  - Be able to pass the employee to the following activities.
      - DeleteEmployeeActivity
      - UpdateEmployeeActivity
- All activities except Main, filter, and list activities must have backward support. (The back arrow in the left side of action bar)
- Main, splash, and list must use single instance, all others must use single task.
