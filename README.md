# Brandon Sanderson's Cosmere

Some books from the Cosmere Universe written by fantasy author Brandon Sanderson

## Content

This project includes a list of some of the sagas in the Cosmere, such as Mistborn or the Stormlight Archive

## Getting Started

The project consists of two documents (xml and dtd). In the xml document there is information about the sagas, for example:

```xml
<brandonsanderson>
    <cosmere>
        <books saga="Elantris">
            <years age="First">
                <book>Elantris 1</book>
            </years>
        </books>
    </cosmere>
</brandonsanderson>
```
In the dtd document is written the necessary data to make the xml work:

```dtd
<!ELEMENT brandonsanderson (cosmere)>
<!ELEMENT cosmere (books+)>
<!ELEMENT books (years+)>
<!ATTLIST books saga CDATA #REQUIRED>
<!ELEMENT years (book+)>
<!ATTLIST years age CDATA #REQUIRED>
<!ELEMENT book (#PCDATA)>
```

## Gratitudes

We have used the next page to gather the information about the Cosmere: [cosmere.es](https://cosmere.es/)

We have also used the next URL to help build the ReadME document: [makeareadme](https://www.makeareadme.com/)

## Authors
- Víctor Gómez Fernández
- David Batista Vega
