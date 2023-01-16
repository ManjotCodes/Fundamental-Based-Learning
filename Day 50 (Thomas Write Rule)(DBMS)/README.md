# Thomas write Rule


Thomas Write Rule provides the guarantee of serializability order for the protocol. It improves the Basic Timestamp Ordering Algorithm.

The basic Thomas write rules are as follows:


If TS(T) < R_TS(X) then transaction T is aborted and rolled back, and operation is rejected.

If TS(T) < W_TS(X) then don't execute the W_item(X) operation of the transaction and continue processing.

If neither condition 1 nor condition 2 occurs, then allowed to execute the WRITE operation by transaction Ti and set W_TS(X) to TS(T).
