# Sequelize



complex where clause

```typescript

const [campaignTicket] = await SeqUserTicket.findAll({
  where: {
    userId: data.id,
    expireAt: {
      [Op.or]: [
        {
          [Op.gte]: new Date(),
        },
        {
          [Op.eq]: null,
        },
      ],
    },
  },
  include: [
    {
      association: SeqUserTicket.associations.ticketInfo,
      where: where(literal(`ticketInfo.type & ${TicketType.캠페인생성}`), '=', String(TicketType.캠페인생성)),
      required: true,
    },
  ],
});
```
