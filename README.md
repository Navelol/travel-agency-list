# Travel Agent Pi-hole Whitelist

A curated list of domains that travel agents need for their work. Keep this as a reference when whitelisting essential travel booking sites, airline systems, car rentals, hotels, and payment processors in Pi-hole.

## Usage

### Reference the List
Use the raw GitHub URL as your go-to reference:
```
https://raw.githubusercontent.com/Navelol/travel-agency-list/main/list.txt
```

Bookmark it and manually add domains to your Pi-hole whitelist as needed.

### Manual Whitelist (Recommended)
In Pi-hole web interface:
1. Go to **Whitelist**
2. Add domains from this list one-by-one as needed
3. Check Pi-hole's **Query Log** to see what's being blocked and reference this list

### Bulk Import (Optional)
If you want to add everything at once via SSH:
```bash
wget https://raw.githubusercontent.com/Navelol/travel-agency-list/main/list.txt
while read domain; do pihole -w "$domain"; done < list.txt
```

## What's Included

- **Airlines**: Delta, United, American, Southwest, JetBlue, etc.
- **Booking Systems**: Sabre, Amadeus, Travelport, CruisingPower
- **Car Rentals**: Avis, Budget, Hertz, Enterprise, National, Alamo
- **Hotels**: Marriott, Hilton, Hyatt, IHG, Choice, Wyndham
- **Cruise Lines**: Carnival, Royal Caribbean, Norwegian, Princess, etc.
- **OTAs**: Expedia, Priceline, Booking.com, Travelocity, Orbitz
- **Payment Processors**: PayPal, Stripe, Google Analytics/Tag Manager

## Contributing

Found a travel site that should be on this list? Open an issue or submit a pull request!

## License

Public domain - use however you want.
