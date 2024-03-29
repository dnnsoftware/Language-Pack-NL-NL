## Pull Requests
All pull requests should be merged into the **develop** branch.

## New version release
When the language pack is ready for a new version:

* Create a branch called release/x.x.x where x.x.x is the version of the release (DNN version)
* Wait a few minutes and you should see a new commit on that branch that updates the manifest automatically with the version taken from that branch.
* When that commit is in, create a pull request from release/x.x.x that targets master, this will automate the packaging and publish the release.
* Optionally another pull request can be created from release/x.x.x targetting develop in order to also update the latest published version on the develop branch


# DNN Language Pack for (nl-NL)

Versions available:
* DNN 09.10.01
* DNN 09.10.00
* DNN 09.07.02
* DNN 09.07.00
* DNN 09.06.02
* DNN 09.06.01
* DNN 09.02.00

## Hoe kun je aan de Nederlandse vertaling bijdragen?

**Uitgangspunt**: om de kwaliteit en consitentie van de vertalingen te bewaken, worden alle bijdragen worden door 2 mensen beoordeeld alvorens ze worden doorgevoerd.

Zorg dat je een (gratis) account hebt op GitHub.

### De minimale werkwijze

1. Fork deze repository (naar je eigen account)
2. Corrigeer binnen GitHub de tekst in de file in je eigen account
3. Maak een Pull Request met je verbetering

### De uitgebreide werkwijze

1. Fork deze repository (naar je eigen account)
2. Clone je eigen (fork) repository naar je lokale schijf
3. Wijzig teksten in de files in je lokale (clone) repository 
4. Controleer met een eigen lokale DNN omgeving of je wijzigingen in orde zijn
5. Commit de wijzigingen in je lokale (clone) repository
6. Push je gecommitte wijzigingen vanuit je (clone) repository naar je (fork) kopie op GitHub
7. Maak een Pull Request met je verbeteringen vanuit je (fork) kopie op GitHub

Als je wijzgingen (Pull Request) uiteindelijk verwerkt is, synchroniseer dan je lokale (clone) repository (Fetch, Merge) en je (fork) kopie op Github (Push). 

De synchronisatie moet je ook doen als anderen bijdragen hebben geleverd die in deze centrale repository zijn verwerkt.

## BELANGRIJK: Common Terms

Om te voorkomen dat de één "U" gebruikt en de ander "Jij" is er een [gids voor taalgebruik](.github/COMMON_TERMS.md). Lees deze s.v.p. door alvorens aan de slag te gaan.

