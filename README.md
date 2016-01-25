# standard-deviation

Simple bit of apex code that I implimented in order for our administrators to give a quality score to evaluations.  The goal is to provide some kinds of statistical scoring methods for quickly evaluating the "quality" of the evaluation / observations of employees work performance without having to peruse the entire document.  

The use a standard deviation does just that.  As an example (for youse who are not statistically-inclined) if you have a hundred evaluation points for which the evaluator scores 1 - 5, a lazy evaluator might just enter a bunch of two's and three's and be done with it.  In doing so, however, the quality scoring (based upon a standard deviation) is going to be absolutely the lowest possible value.  And this is meant to inform a reviewer that the evaluation may have been done hastily or haphazardly.

In this case, the target code 'DSPevalScoring.getStdDev(dsp_eval__c arec, decimal mean)'  takes the eval record, unwinds all of the score values from the record and performs the calculations required to produce the StdDev and returns this val to the calling method. 
