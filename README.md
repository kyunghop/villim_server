# villim_server

Server APIs

**Welcome**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
</table>


**Verify 1 (email)**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/login-email</td>
    <td>email (1)</td>
    <td>success (1)</td>
  </tr>
</table>


**Verify 2 (phone)**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/login-phone</td>
    <td>phonenumber (1)</td>
    <td>success (1)</td>
  </tr>
</table>


**My Room	**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/myroom</td>
    <td> -</td>
    <td>room_id, room_name, num_guest, room_type, num_bed, num_bath, date_begin, date_end (8)</td>
  </tr>
</table>


**Passcode**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/change-passcode</td>
    <td>old_passcode, new_passcode, confirm_passcode (3)</td>
    <td>success (1)</td>
  </tr>
</table>


**Home**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/available-rooms</td>
    <td>-</td>
    <td>for each room: 
room_id, room_name, num_guest, room_type, num_bed, num_bath, tumbnail_url, room_price (8)  </td>
  </tr>
</table>


**Room Detail 1**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-info</td>
    <td>room_id (1)</td>
    <td>room_id, room_name, num_guest, room_type, num_bed, num_bath, tumbnail_url, room_price, room_size, room_deposit, price_single, price_double, price_triple, room_liked (14) </td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/like-room</td>
    <td>room_id (1)</td>
    <td>success (1)</td>
  </tr>
</table>


**Room Detail 2**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-address</td>
    <td>room_id (1)</td>
    <td>room_id, room-address (2)</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-facility</td>
    <td>room_id (1)</td>
    <td>room_id, room-facility (2)</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-policy</td>
    <td>room_id (1)</td>
    <td>room_id, room-policy (2)</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-cancellation</td>
    <td>room_id (1)</td>
    <td>room_id, room-cancellation (2)</td>
  </tr>
</table>


**Reserve**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/room-available</td>
    <td>room_id, date_begin, date_end (3)</td>
    <td>room_id, available_dates (2)</td>
  </tr>
</table>


**Finish Reserve**

<table>
  <tr>
    <td>Type</td>
    <td>URL</td>
    <td>Parameters</td>
    <td>Response</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/reserve</td>
    <td> room_id, date_begin, date_end (3)</td>
    <td>room_id, success (2)</td>
  </tr>
</table>


