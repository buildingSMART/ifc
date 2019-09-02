_IfcEvent_ may be contained within an _IfcTask_ using the _IfcRelNests_ relationship. The event is considered active during the time period of the enclosing task (including any assigned _IfcWorkCalendar_); that is such event may be triggered within the task time period but not outside of it. As an _IfcEvent_ is considered to be atomic, no use is anticipated for nesting processes inside the event.