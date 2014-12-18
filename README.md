# gSchool `collection_select` Practice

Add the associations and collection_select methods necessary to make this work.

<%= form_for #@employment do |f| %>

  <div class="well">
    <p>
      <strong>Instructions</strong>
    </p>

    <ul>
      <li>Give all of the dropdowns a class of "form-control"</li>
      <li>Make the person dropdown have no blank options</li>
      <li>Make the organization dropdown have a blank option</li>
      <li>Make the job title dropdown have a blank option, but the user sees "Select a title, yo!"</li>
    </ul>

    <p>
      <strong>Bonus!</strong>
      <br>Make the location dropdown have a blank option, but make that option go away
      after a user has selected something.  So on the "new" page there's a blank option, but on the
      edit page there's no blank option.
    </p>
  </div>

  <div class="form-group">
    <%= f.label :person_id %>
    <em>Add the people dropdown here</em>
  </div>

  <div class="form-group">
    <%= f.label :organization_id %>
    <em>Add the organizations dropdown here</em>
  </div>

  <div class="form-group">
    <%= f.label :job_title_id %>
    <em>Add the job titles dropdown here</em>
  </div>

  <div class="form-group">
    <%= f.label :location_id %>
    <em>Add the locations dropdown here</em>
  </div>

  <p>
    <%= f.submit class: "btn btn-primary" %>
  </p>

<% end %>
