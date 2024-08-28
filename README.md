# range_accrual_note


A Range Accrual Note is a type of structured financial product that pays interest based on how often a reference rate (such as LIBOR) stays within a predefined range during the life of the note. These notes are attractive to investors who believe that interest rates will remain within a certain range over the investment period.


Notional Amount (N): The principal amount on which interest is calculated.
Coupon Rate (C): The fixed annual interest rate that would be paid if the reference rate remains within the specified range every day.
Reference Rate (R_t): The underlying rate (e.g., LIBOR) observed on each day t.
Lower Bound (L): The lower limit of the range for the reference rate.
Upper Bound (U): The upper limit of the range for the reference rate.
Observation Period: The total number of days (n) during which the reference rate is observed.
Days in Range (d): The number of days during the observation period that the reference rate stays within the range [L, U].


The interest accrued by the Range Accrual Note is proportional to the number of days the reference rate stays within the specified range [L, U]. The total interest payment at the end of the observation period is calculated as:
Interest = N * C * (d / n)
Where:
d is the number of days the reference rate R_t stays within the range [L, U].
n is the total number of observation days.


Daily Observation: Each day, the reference rate R_t is observed and checked to see if it falls within the range [L, U]. If it does, that day counts toward the total number of days in range d.
d = sum_{t=1}^{n} 1,  if  L <= R_t <= U
If the reference rate R_t is outside the range [L, U] on a particular day, that day does not count toward d.

Interest Calculation: At the end of the observation period, the total interest accrued is based on the proportion of days d/n that the reference rate stayed within the range:
Interest = N * C * (d / n)
This formula implies that the interest payment will be lower if the reference rate frequently falls outside the range [L, U].
