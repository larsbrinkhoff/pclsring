### Demo of PC losering

1. Assemble PCLSR DEMO.
2. Load into DDT, and start with <kbd>$0G</kbd>.
3. Single step with <kbd>^N</kbd> until the .IOT system call.
4. Observe A is initially -100,,BUF.
5. Type <kbd>$P</kbd> to execute the .IOT.
6. Type <kbd>ABCDE</kbd> and then <kbd>^Z</kbd> to interrupt .IOT.
7. Observe job still pointing to the .IOT call, and type <kbd>A/</kbd>
   to observe A is now -77,,BUF+1.
8. Proceed with <kbd>$P</kbd> type <kbd>12345^C</kbd>
9. Observe A is now -76,,BUF+2, and contents of BUF is ABCDE12345.
