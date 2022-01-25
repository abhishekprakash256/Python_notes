## Python Tornado 

### Sub Heading 

- pip install tornado 

#### Imp Imports

```python
import tornado.web
import tornado.ioloop 
```

### Notes

- The main code to start the Application 

```python
if __name__ == "__main__":  #made a list of the tuple that has functionality
	app = tornado.web.Application([
		(r"/", basicRequestHandler),
		(r"/blog", staticRequestHandler),
		(r"/isEven",isEvenRequestHandler),
		(r"/tweet/([0-9]+)", isTweetRequestHandler)
		])
```

- Initializing the port and the app

  ```python
  	app.listen(8881)
  	print("The port started")
  	tornado.ioloop.IOLoop.current().start()
  ```

- Class for the functionality 

  ```python
  class isEvenRequestHandler(tornado.web.RequestHandler):
  	def get(self):
  		n = int(self.get_argument("n"))
  		r= "even" if n % 2 == 0 else "odd"
  		self.write("The number " + str(n) + " is " + r)
  ```

### Full code example 

```python
"""
starting the torando API
"""
import tornado.web 
import tornado.ioloop

class basicRequestHandler(tornado.web.RequestHandler):
	def get(self):

		self.write("Hell")

class isTweetRequestHandler(tornado.web.RequestHandler):
	def get(self,id):

		self.write("The quesry that is given is " + id)


class isEvenRequestHandler(tornado.web.RequestHandler):
	def get(self):
		n = int(self.get_argument("n"))
		r= "even" if n % 2 == 0 else "odd"
		self.write("The number " + str(n) + " is " + r)


class staticRequestHandler(tornado.web.RequestHandler):
	def get(self):
		self.render("index.html")

if __name__ == "__main__":
	app = tornado.web.Application([
		(r"/", basicRequestHandler),
		(r"/blog", staticRequestHandler),
		(r"/isEven",isEvenRequestHandler),
		(r"/tweet/([0-9]+)", isTweetRequestHandler)

		])

	app.listen(8881)
	print("The port started")
	tornado.ioloop.IOLoop.current().start()


```

