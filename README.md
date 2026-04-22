# restaurant-table-booking-system
package com.restaurant.entity;

import jakarta.persistence.*;
import java.time.LocalDate;
import java.time.LocalTime;

@Entity
public class Booking {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String customerName;
    private Long tableId;
    private LocalDate date;
    private LocalTime time;

    public Long getId() { return id; }
    public String getCustomerName() { return customerName; }
    public Long getTableId() { return tableId; }
    public LocalDate getDate() { return date; }
    public LocalTime getTime() { return time; }

    public void setId(Long id) { this.id = id; }
    public void setCustomerName(String customerName) { this.customerName = customerName; }
    public void setTableId(Long tableId) { this.tableId = tableId; }
    public void setDate(LocalDate date) { this.date = date; }
    public void setTime(LocalTime time) { this.time = time; }
}
