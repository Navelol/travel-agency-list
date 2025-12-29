# Travel Agent Pi-hole Whitelist

A curated list of domains that travel agents need for their work. Use this to whitelist essential travel booking sites, airline systems, car rentals, hotels, and payment processors in Pi-hole.

## Usage

### Manual Import (One-by-one)
In Pi-hole web interface, go to **Whitelist** and add each domain from the list.

### Bulk Import via SSH
1. SSH into your Pi-hole
2. Download the list:
```bash
wget https://raw.githubusercontent.com/YOUR-USERNAME/YOUR-REPO-NAME/main/travel-agent-pihole-whitelist.txt
```
3. Import all domains:
```bash
while read domain; do pihole -w "$domain"; done < travel-agent-pihole-whitelist.txt
```

## What's Included

- **Airlines**: Delta, United, American, Southwest, JetBlue, etc.
- **Booking Systems**: Sabre, Amadeus, Travelport, CruisingPower
- **Car Rentals**: Avis, Budget, Hertz, Enterprise, National, Alamo
- **Hotels**: Marriott, Hilton, Hyatt, IHG, Choice, Wyndham
- **Cruise Lines**: Carnival, Royal Caribbean, Norwegian, Princess, etc.
- **OTAs**: Expedia, Priceline, Booking.com, Travelocity, Orbitz
- **Payment Processors**: PayPal, Stripe

## Contributing

Found a travel site that should be on this list? Open an issue or submit a pull request!

## License

Public domain - use however you want.
