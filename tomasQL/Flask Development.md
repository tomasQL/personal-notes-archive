### Flask micro-framework

**Installing VENV**
  
    python3 -m pip install --user virtualenv  
    
**Setting up virutal enviroment**
  
    python3 -m venv <folder name to the venv>
	    normally .venv or project name venv
    *add venv in file .gitignore
      
    source env/bin/activate  
    deactivate  
  
**Installing Flask**
  
    pip install Flask
  
**Run Flask app**
  
    flask -app <nameapp> run


**Remember: ORM's**

ORM makes writing SQL queries easier. We write it in an object-oriented  
language, and then the ORM automatically translates ir to SQL and retrieve  
the result in the form of objects.

**Models**
*One to many relationship*

	class Employee(db.Model):
		employee_id = db.Column(db.Integer, primary_key=True)
		first_name = db.Column(db.String(50), nullable=False)
		last_name = db.Column(db.String(50), nullabe=False)
		
	class Department(db.Model):
		name = db.Column(db.String(50), primary_key=True, 
			nullable=False)
		location = db.Column(db.String(120), nullable=False)
		employees = db.relationship('Employee', backref='department')

We passed 'Employee' as an argument to the function to specify  with wich model we want  
to create this relationship the back-reference means is that virtual variable department will   
be created in the Employee table. This way, we can refer to it by employee.department.  
We already have a FK, however, that only give us the name column of the department row.  
Backref will act as a virtual column in the user table containing the whole row of the  
department.