# DNS Violations
List of DNS violations by implementations, software and/or systems

## About
This _List_ consists of DNS Violation Entries (_DVE_'s) that describes known
violations to the DNS protocol by implementations, software and/or systems.

## Purpose
The purpose of the _List_ is to better understand how wrongfully the DNS
protocol is used out in the wild in order to try and make it better.
There is also a great gain for implementers to verify that they can handle
wrong DNS correctly.

## Community based
The _List_ is driven by the community for the community, anyone can send in
a violation and a team of community members will review and accept or reject
the violation, this team in called _Maintainers_.  Anyone can request to join
the _Maintainers_ team and <acceptance method TBD>.

## Violation
An implementation, software and/or system is considered to be in violation
to the DNS protocol when it does not strongly conform to the current DNS
RFCs.  Violations can also include updated or obsolete DNS RFCs.

## Submission
Anyone can submit a DNS violation and request a _DVE_, this is done as a
pull request or an issue.

### Format
The format is Markdown with the following suggested headers, which are not
strict but should at least have short and long description.  Metadata may be
included at the end of headers, together under `Metadata` header or at the
end of the file.

```
# DVE-<YEAR>-<NUMBER>: <short description>

## Description

<long description>

## Evidence

<the evidance that the violation occurred, can be shell output, tcpdump etc>

## Proposed fix

<how to, hopefully, fix it>

## Workaround

<if there are any>

## DNS Operator/Vendor Response

<if there's any>

## Metadata

Submitter: <may be used if the source is not a commit>
Submit-Date: <date>
Report-Date: <date> <upstream-contact>
Fixed-Date: <date>
Tags: <free form tags for the DVE as a comma seperated list>
<meta-data>: <value>
```

## DVE Allocation
_DVE_ are allocated sequentially starting from the number 1 using the format
`DVE-<YEAR>-<NUMBER>`.  The number is allocated on a first-come-first-served
bases via pull requests or by the _Maintainers_ for an issue.  The
_Maintainers_ may reserve a number for an issue by updated the title of the
issue with the full _DVE_ and also add a comment addressed to
`@DNS-OARC/dve-maintainers` that it has been reserved.  Collisions are
rejected/asked to be updated.
