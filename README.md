#Read me file for the website
here are the sql queries i have used:

-- Allow the website to update the buzzer ON/OFF status
create policy "Allow host to update buzzer status"
on quiz_sessions
for update
to anon
using (true)
with check (true);
