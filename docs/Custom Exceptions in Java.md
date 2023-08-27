# [[Custom Exception]]s in Java

- How to create?

    Create a class WhateverException which extends Exception

- How to return your custom message while throwing exception?

    Pass the message you want to show as a String to the Exception (or super).

- Are custom exceptions checked or unchecked?

    If you want it to be checked, extend Exception. If you want it to be unchecked, extend RuntimeException.
