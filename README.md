# Filtering of signal_input,

Input and Output Signals: The input signal x and the output signal y are defined. These are the signals that you will be working with.

Filter Requirements: The order of the filter and the sample rate are defined. The lowcut and highcut variables define the desired cutoff frequencies of the filter.

Create the Filters: The butter function is used to create the Low Pass, High Pass, and Band Pass filters. The output of the butter function are the filter coefficients which are used in the next step.

Apply the Filters: The filter function is used to apply each of the filters to the input signal x. This results in three filtered output signals: ylp (Low Pass), yhp (High Pass), and ybp (Band Pass).

Compare the Filtered Outputs: The xcorr function is used to calculate the correlation between each of the filtered output signals and the given output signal y. This results in three correlation results: corr_ylp, corr_yhp, and corr_ybp.

Identify the Best Match: The max function is used to identify which correlation result is the largest. This tells us which filtered output best matches the given output signal. The result is then displayed using the disp function.
