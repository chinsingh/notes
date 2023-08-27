# Backdoor Injection

Injection done using friend class.

```abap
CLASS … DEFINITION … .
  PRIVATE SECTION.
    DATA m_cash_provider TYPE REF TO if_cash_provider.
    …
ENDCLASS.
```

```abap
CLASS ltc_get_amount_in_coins DEFINITION DEFERRED.
CLASS cl_money_machine DEFINITION
    LOCAL FRIENDS ltc_get_amount_in_coins.

CLASS ltc_get_amount_in_coins DEFINITION FOR TESTING … .
…
ENDCLASS.

CLASS ltc_get_amount_in_coins IMPLEMENTATION.
  METHOD setup.
    "given
    m_cut = NEW #( ).
    m_cut->m_cash_provider = NEW ltd_cash_provider( ).
  ENDMETHOD.
ENDCLASS.
```
