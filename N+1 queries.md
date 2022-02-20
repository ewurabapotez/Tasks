##### Increase performance in long running endpoints

`notifiers ... Potential n+1 query detected on Booking.service`

Possible soln: Booking.objects.all().select_related('service')


`notifiers ... Potential n+1 query detected on Post.author`

Possible soln: Post.objects.all().select_related('author')


`notifiers ... Potential n+1 query detected on Invoice.bill_to`

Possible soln: Invoice.objects.all().select_related('bill_to')


`notifiers ... Potential n+1 query detected on Transaction.payment_method`

Possible soln: Transaction.objects.all().select_related('payment_method')


`notifiers ... Potential n+1 query detected on Profile.user`

Possible soln: Profile.objects.all().select_related('user')