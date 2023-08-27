# Skip Validations while creating SE

For certain use cases, validations are skipped during [[Service Execution Creation]].

This is taken care of by the `/A1SSPC/CL_SE_SKIP_VALIDATION` API which is a [[Singleton]] class (kind of - the constructor is not private).

The class has a flag `mv_skip_validation_toggle` which tells whether validations are to be skipped or not. Since the flag has to be checked from multiple places, once set, it should hold that value consistently. This is why the class needs to be a singleton.

The singleton instance `mo_skip_validation` is fetched using `get_instance` [[Static Method]].

After that you can use `activate_validation` or `deactivate_validation` method to either toggle the switch on and off or you check if the flag is on using `is_skip_validation_active` method.

Example:

From [[Service Execution Creation API]] `/A1SSPC/IF_HANDLE_REQUEST~CREATE_FOLLOW_UP_OBJS` line 18

```abap
/a1sspc/cl_se_skip_validation->get_instance( )->activate_validation( ).
```

## References
