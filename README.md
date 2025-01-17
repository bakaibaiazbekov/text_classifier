# text_classifier
I analyze the card sort with scaling and clustering to create the attached xlsx file with multiple worksheets (wks).


“Output” wks: 
    x,y coordinates of each item in columns A & B. 
    Cols C through M is cluster membership for each item for cluster solutions 15 through 5.     
    Cols N & O are item numbers and item text.
    when the cards are sorted, they make labels, then compute distance. 

“clu5 top labels” wks: 
     when a person sorts the cards, they add a label or name to each of their groupings. 
     I compute the location of each label and identify the labels closest to the center of each cluster. 
     So this wks has 25 labels, five labels that are closest to the center of each of five clusters. 
     Note that center here is defined as the the average x, average y for all items in a cluster. 
     Center is not the geometric center that would be defined by the average x,y for the boundary items. 
     I provide the labels because this is text that could also contribute to describing the cluster along with the items. 
     The remaining wks (e.g. clu6 top labels) are similarly organized for the other cluster solutions.

The wks “unsorted”:
      are the items that were NOT included in the card sort. 
      I would like this project to develop an approach to assigning these unsorted items to clusters.
      In any given project I use “output” wks to determine the optimal cluster solution to 
      use for reporting. 
      I would like the algorithm for this project to apply to any cluster solution I choose.
      I also recognize that an algorithm may perform better or worse depending on the number 
      of clusters. 
      For example, using the 12 cluster solution means that there are few words that can be
      sampled from each cluster to creating the training model than would be the case for the
      5 cluster solution. 
      On the other hand, the 12 cluster solution would have clusters with more precise
      meaning and the 5 cluster solution would have more ambiguous meaning. As such I am not
      sure how the number of clusters would affect the outcome and look to your expertise.
