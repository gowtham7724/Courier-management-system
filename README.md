# Courier Management System (CMS)

## Project Overview
A Salesforce-based Courier Management System designed to centralize and automate courier operations including shipment booking, tracking, delivery-agent assignment, notifications, billing, and reporting.

## Problem Statement
Manual processes and disconnected systems can cause delayed updates, poor visibility, delivery-agent assignment conflicts, manual follow-ups, limited performance analytics, and difficulties coordinating multiple branches.

## Purpose
- Manage customer information
- Book and track shipments
- Assign delivery agents
- Update shipment status
- Generate invoices
- Provide reports and dashboards
- Support multi-branch courier operations

## Technology Stack
| Area | Technology |
|---|---|
| UI | Salesforce Lightning |
| Business Logic | Salesforce Flows |
| Database | Salesforce Objects |
| Automation | Validation Rules, Flows |
| Security | Profiles, Roles |
| Reporting | Reports & Dashboards |

## Main Modules
1. Customer Management
2. Shipment Management
3. Delivery Agent Management
4. Branch Management
5. Delivery Updates
6. Invoice Management
7. Reports
8. Dashboards
9. Security and User Management

## Salesforce Objects
- Customer__c
- Shipment__c
- Delivery_Agent__c
- Branch__c
- Delivery_Update__c
- Invoice__c

## Relationships
- Customer → Shipment: Lookup
- Shipment → Delivery Agent: Lookup
- Delivery Agent → Branch: Lookup
- Delivery Update → Shipment: Master-Detail
- Invoice → Shipment: Lookup

## Shipment Status
- Booked
- In Transit
- Out for Delivery
- Delivered
- Cancelled

## Delivery Agent Status
- Active
- Inactive
- On Leave

## Invoice Payment Status
- Paid
- Unpaid
- Pending

## Automation
A record-triggered Salesforce Flow named Auto_Update_Shipment_Status updates the related shipment status whenever a Delivery Update record is created.

## Security
The project defines role/profile access for Courier Admin, Branch Manager, Delivery Agent, and Customer Support. The role hierarchy places Courier Admin at the top, with Branch Manager below it and Delivery Agent / Customer Support under Branch Manager.

## Reports
- Shipment Tracking Report
- Customer Summary Report
- Agent Performance Report
- Shipment Status Summary
- Revenue by Branch Report

## Dashboard
The Courier Management Dashboard includes Shipment Status Overview, Agent Performance, and Revenue by Branch.

## Testing
The project documentation describes testing for record creation, validation rules, status updates, flow automation, invoice generation, and dashboard visualization.

## Advantages
- Centralized data
- Automated workflows
- Real-time reporting

## Disadvantages
- Salesforce dependency
- Requires initial configuration effort

## Future Scope
- Mobile tracking application
- GPS integration
- SMS notifications
- AI-based delivery optimization

## Platform
Salesforce
