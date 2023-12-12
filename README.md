How to start it
Interactive Mode
$ ./console.py
Now you are on interactive mode and you will see the prompt (hbnb) input a command:

(hbnb) create User
the id of the created model will be visible in the standard output, if you do:

(hbnb) show User [id]
All the attributes of the created model will be in your screen.

use:

(hbnb) help
For a list of usable commands, to exit press Ctrl+D or type the command quit.

Non-Interactive Mode
The console can also be used in non-interactive mode:

$ echo "create User" | ./console.py

$ echo "help" | ./console.py
The program will create a file called: file.json whenever you create a new model, it'll be store in the top folder.

Available classes
Class name	Attributes
BaseModel	id, created_at, updated_at
User	email, password, first_name, last_name
State	name state_id
City	name
Amenity	name
Place	city_id user_id name description number_rooms number_bathrooms max_guest price_by_night latitude``longitude amenity_ids
Review	place_id user_id text
every model inherits attributes from BaseModel
