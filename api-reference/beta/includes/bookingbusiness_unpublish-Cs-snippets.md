
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
	.Unpublish(bookingBusiness)
	.Request()
	.PostAsync()

```