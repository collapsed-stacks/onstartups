## Working @ Startup. Need help reading their most recent SEC Filing

- posted by: [user19426](https://stackexchange.com/users/-1/19426-user19426) on 2012-08-27
- tagged: `investors`, `venture-capital`, `stocks`
- score: 1

Our Company just raised another round of funding (5MM). I took a peak at the SEC filing and it was confusing. See below:

Total Offering Amount $18,500,000 USD  Total Amount Sold $9,777,138 USD Total Remaining to be Sold $8,722,862 USD

Clarification of Response (if Necessary): Warrants with an aggregate exercise price of approximately $4,933 were issued in connection with the financing; such amount is not included in the above figure.

What does this mean?

Note: I intentionally omitted the link to the actual filing itself.


[Edit] Here's pretty much the rest of the filing in XML format

    <offeringData>
        <issuerSize>
            <revenueRange>Decline to Disclose</revenueRange>
        </issuerSize>
        <federalExemptionsExclusions>
            <item>06</item>
        </federalExemptionsExclusions>
        <typeOfFiling>
            <newOrAmendment>
                <isAmendment>false</isAmendment>
            </newOrAmendment>
            <dateOfFirstSale>
                <value>2012-08-10</value>
            </dateOfFirstSale>
        </typeOfFiling>
        <durationOfOffering>
            <moreThanOneYear>false</moreThanOneYear>
        </durationOfOffering>
        <typesOfSecuritiesOffered>
            <isEquityType>true</isEquityType>
            <isOptionToAcquireType>true</isOptionToAcquireType>
        </typesOfSecuritiesOffered>
        <businessCombinationTransaction>
            <isBusinessCombinationTransaction>false</isBusinessCombinationTransaction>
            <clarificationOfResponse></clarificationOfResponse>
        </businessCombinationTransaction>
        <minimumInvestmentAccepted>0</minimumInvestmentAccepted>
        <salesCompensationList></salesCompensationList>
        <offeringSalesAmounts>
            <totalOfferingAmount>18500000</totalOfferingAmount>
            <totalAmountSold>9777138</totalAmountSold>
            <totalRemaining>8722862</totalRemaining>
            <clarificationOfResponse>Warrants with an aggregate exercise price of approximately $4,933 were issued in connection with the financing; such amount is not included in the above figure.</clarificationOfResponse>
        </offeringSalesAmounts>
        <investors>
            <hasNonAccreditedInvestors>false</hasNonAccreditedInvestors>
            <totalNumberAlreadyInvested>4</totalNumberAlreadyInvested>
        </investors>
        <salesCommissionsFindersFees>
            <salesCommissions>
                <dollarAmount>0</dollarAmount>
            </salesCommissions>
            <findersFees>
                <dollarAmount>0</dollarAmount>
            </findersFees>
            <clarificationOfResponse></clarificationOfResponse>
        </salesCommissionsFindersFees>
        <useOfProceeds>
            <grossProceedsUsed>
                <dollarAmount>0</dollarAmount>
            </grossProceedsUsed>
            <clarificationOfResponse></clarificationOfResponse>
        </useOfProceeds>
    </offeringData>

[Edit #2] This is the previous filing (2010), a bit more revealing. Convertible Debt?

     <offeringData>
        <issuerSize>
            <revenueRange>Decline to Disclose</revenueRange>
        </issuerSize>
        <federalExemptionsExclusions>
            <item>06</item>
        </federalExemptionsExclusions>
        <typeOfFiling>
            <newOrAmendment>
                <isAmendment>false</isAmendment>
            </newOrAmendment>
            <dateOfFirstSale>
                <value>2010-09-01</value>
            </dateOfFirstSale>
        </typeOfFiling>
        <durationOfOffering>
            <moreThanOneYear>false</moreThanOneYear>
        </durationOfOffering>
        <typesOfSecuritiesOffered>
            <isOptionToAcquireType>true</isOptionToAcquireType>
            <isOtherType>true</isOtherType>
            <descriptionOfOtherType>convertible debt</descriptionOfOtherType>
        </typesOfSecuritiesOffered>
        <businessCombinationTransaction>
            <isBusinessCombinationTransaction>false</isBusinessCombinationTransaction>
            <clarificationOfResponse></clarificationOfResponse>
        </businessCombinationTransaction>
        <minimumInvestmentAccepted>0</minimumInvestmentAccepted>
        <salesCompensationList></salesCompensationList>
        <offeringSalesAmounts>
            <totalOfferingAmount>9210635</totalOfferingAmount>
            <totalAmountSold>4210635</totalAmountSold>
            <totalRemaining>5000000</totalRemaining>
            <clarificationOfResponse>In addition, warrants for purchase of capital stock valued at $1,842,127.</clarificationOfResponse>
        </offeringSalesAmounts>
        <investors>
            <hasNonAccreditedInvestors>false</hasNonAccreditedInvestors>
            <totalNumberAlreadyInvested>1</totalNumberAlreadyInvested>
        </investors>
        <salesCommissionsFindersFees>
            <salesCommissions>
                <dollarAmount>0</dollarAmount>
            </salesCommissions>
            <findersFees>
                <dollarAmount>0</dollarAmount>
            </findersFees>
            <clarificationOfResponse></clarificationOfResponse>
        </salesCommissionsFindersFees>
        <useOfProceeds>
            <grossProceedsUsed>
                <dollarAmount>0</dollarAmount>
            </grossProceedsUsed>
            <clarificationOfResponse></clarificationOfResponse>
        </useOfProceeds>
    </offeringData>


## Answer 41637

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-08-27
- score: 2

It means that the Company authorized the sale of $18.5M in securities (not clear what securities), and has so far sold $9.78M.  

As part of the offering, the Company sold warrants to buy its stock.  A warrant is like an option -- it gives you the right to buy the stock at a set exercise price at a later time.  In this case, if you add up the total exercise prices of all the warrants, it's equal to $4,933.  They didn't include that in the $18.5M number because they only get it when somebody exercises the warrant.

I presume that you're looking at a Form D filing.  As the offering proceeds, the company may update the filing to increase those amounts.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
