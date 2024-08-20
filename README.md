READ a, b, c, d, e, f

D = a*e - b*d

IF D = 0 THEN
    IF (a*f - c*d) != 0 OR (b*f - c*e) != 0 THEN
        PRINT "No solution (parallel lines)"
    ELSE
        PRINT "Infinitely many solutions"
    ENDIF
ELSE
    x = (c*e - b*f) / D
    y = (a*f - c*d) / D
    PRINT "Solution: x =", x, "y =", y
ENDIF

END
