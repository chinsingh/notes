# Accessing [[Static]] members using objects

Its possible to write f.classMethod(). It is legal but a bad idea, since it causes confusion. The instance is not important in case of class methods. Only the declared type of 'f' matters.

Its better to write Foo.classMethod() or Bar.classMethod(). This not only makes it clear which class method you would like to call. But also, that it is indeed a class method which you're calling.

Of course, all this could be avoided by simply trying to not overide your static methods. You know, because [[Static Methods can't be overridden]]
