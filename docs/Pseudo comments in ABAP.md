# Pseudo comments in ABAP

Pseudo comments are used to provide information to check and test procedures.

For example, you can ignore a certain ATC check using pseudo comments.

Pseudo comments are mostly obsolete though and are being replaced by [[Pragmas in ABAP]].

Example:

```abap
METHOD get_sources.
     SELECT source, textlong
       INTO TABLE @rt_source
       FROM tb006
       WHERE spras = @sy-langu. "#EC CI_SUBRC
ENDMETHOD.
```

## References

- [What are pragmas and pseudo comments in ABAP - SAP blogs](https://blogs.sap.com/2019/09/11/what-are-pragmas-and-pseudo-comments-in-abap/)
- [ATC Pseudo comments list](https://abapblog.com/articles/tips/124-atc-pseudo-comments-list)
