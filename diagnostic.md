# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
Backend is necessary for webpages because it allows for interactions among different users on different devices, and allows data to be saved over time. For example, if two people are using a webpage, they have two different copies and can never interact with each other unless there is backend. Similarly, you would need backend if you want to save your game and come back to the same place later.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
We use 'serializers' that act like the View layer.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Model (M)
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
GET (all), GET (single), PATCH, POST, DELETE, PUT
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- User fires 'GET' request for 'people/1'
- API sends request to Controller
- Controller parse user request, sends request to Model
- Model retrieves people item with index 1 from the peoples table of the people database, sends back data to Controller
- Controller sends data to View
- View formats the data, sends it back to Controller
- Controller sends it back to API
- API sends back requested data to Browser (client)
```

What is the command to generate a new rails-api app?

```bash
bin/rails generate
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
db:drop
db:create
db:migrate
db:seed
db:example
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:text age:integer
```
