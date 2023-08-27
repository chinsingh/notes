# Transactions are performed on buffer

All operations in a transaction are performed on a buffer which is a copy of the database or record. So even if a transaction fails any stage, the buffer is removed and the database remains unaffected. If it is successful the data will be copied.
