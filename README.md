<h2>E-Vent</h2>

E-Vent is an event planning app.  Users can submit an event, and manage their attendance at events.

Models in use for this app are:
  User -< Attendance >- Event

E-Vent uses BCrypt to authenticate users.  

A logged-in user can:
<ul>
  <li>Persist their logged-in state through a page refresh</li>
  <li>Create an event with details</li>
    <li>(CRUD actions on Attendance using RESTful routes)</li>
    <ul>
   <li> Register for an existing event, along with the total number of attendees they plan to bring</li>
   <li> Have their registration displayed to all users</li>
   <li> Update their number of attendees</li>
   <li> Cancel their registration</li>
   <li> Display all of the events for which they are registered</li>
   </ul>
  <li>Log out of the app</li>
</ul>

Users cannot update or destroy the attendances of other users.

Validation and controller errors are passed to the frontend and displayed to users.






