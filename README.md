School Management Application
This is a school management application that allows for the creation and management of schools, courses, batches, and students. It provides a flexible and secure platform for educational organizations with different user types and their respective capabilities.

Features
User Types:

Admin: Has full control over the system and can create schools and School Admins.
School Admin: Can update information about the school, create courses and batches, add students to batches, and approve/deny enrolment requests made by students.
Student: Can raise a request to enroll in a batch, view classmates, and track progress.
Database: The application uses SQLite as the database.

Technology Stack:

Ruby version: 3.0.3p157
Rails version: 7.0.4.3
Gems:
bcrypt (version 3.1.7) for token generation and authentication.
jwt (version 2.2.3) for JSON Web Token authentication.
pundit (version 2.3) for authorization.
kaminari for pagination.
fast_jsonapi for fast and easy JSON serialization.
slim-rails for using the Slim template engine.
bootstrap (version 5.1.3) for a responsive user interface.
API Support: The application is available as an API, providing a flexible way to interact with the system.

Installation
Follow these steps to set up the application:

Clone the repository: git clone <repository-url>

Install the required gems: bundle install

Set up the database and seed data:

bash
Copy code
rails db:setup
rails db:seed
This will create the database, load the schema, and populate it with default roles (Admin, SchoolAdmin, Student).

Start the server: rails server

Testing
The application uses RSpec for testing.

To run all the tests, use the following command:

bash
Copy code
bundle exec rspec
This will execute the full test suite, including model, serializer, and request specs, and provide you with the test results.

You can also run specific types of specs. For example:

To run model specs:

bash
Copy code
bundle exec rspec spec/models
To run serializer specs:

bash
Copy code
bundle exec rspec spec/serializers
To run request specs:

bash
Copy code
bundle exec rspec spec/requests
Feel free to explore the spec directory to see the available spec files and customize the test suite according to your needs.

Contributors
This application is maintained by [Your Name]. Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

License
This project is licensed under the MIT License.
